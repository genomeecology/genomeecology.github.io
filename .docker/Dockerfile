# start with official ruby docker image as base
FROM ruby:3.1-bookworm

# set working directory within container
WORKDIR /usr/src/app

# pull in ruby (jekyll) and python (cite process) package info
COPY Gemfile Gemfile.lock _cite/requirements.txt ./

# install ruby packages
RUN VERSION=$(grep -A 1 'BUNDLED WITH' Gemfile.lock | tail -n 1 | xargs); \
    gem install bundler --version ${VERSION} && \
    bundle _${VERSION}_ install

# install python and create an isolated environment for its dependencies
RUN apt-get update && apt-get install -y --no-install-recommends python3 python3-venv && \
    python3 -m venv /opt/venv && \
    rm -rf /var/lib/apt/lists/*

ENV PATH="/opt/venv/bin:$PATH"

# install python packages
RUN pip install --no-cache-dir --upgrade --requirement requirements.txt && \
    pip install --no-cache-dir "watchdog[watchmedo]==3.0.0"

# ports used by jekyll
EXPOSE 4000
EXPOSE 35729

# run jekyll and cite process
COPY .docker/entrypoint.sh /var
CMD [ "/var/entrypoint.sh" ]
