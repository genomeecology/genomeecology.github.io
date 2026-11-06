
  ![on-push](../../actions/workflows/on-push.yaml/badge.svg)
  ![on-pull-request](../../actions/workflows/on-pull-request.yaml/badge.svg)
  ![on-schedule](../../actions/workflows/on-schedule.yaml/badge.svg)

  # genomeecology's Website

  Visit **[genome-ecology.com](https://genome-ecology.com)** 🚀

  _Built with [Lab Website Template](https://greene-lab.gitbook.io/lab-website-template-docs)_

  ## Citation cache

  The Docker preview stores its citation cache in the Docker volume
  `lab-website-citation-cache`, separate from the bind-mounted website files.
  The cache contains only results that can be fetched again.

  If a citation build reports `database disk image is malformed`, stop the
  preview and any other citation processes before clearing the affected cache:

  - For the Docker preview, run `docker volume rm lab-website-citation-cache`.
    The next run of `.docker/run.sh` creates a fresh cache.
  - For a citation process run directly on the host, rename or delete
    `_cite/.cache`. It will be recreated on the next run.

  The first run with a fresh cache may take longer and requires network access.
