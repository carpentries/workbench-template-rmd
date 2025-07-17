FROM carpentries/workbench-docker:latest

RUN Rscript -e 'sandpaper::use_package_cache(prompt = FALSE)'

COPY renv/profiles/lesson-requirements/renv.lock .
RUN Rscript -e 'renv::restore(prompt = FALSE)'
