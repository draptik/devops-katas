# DevOps Katas

Just an idea: coding katas are a good way to learn coding.

What about DevOps katas?

Practice using tools such as

- git: github, gitlab, etc
- docker, docker-compose
- etc

## Kata: Hugo

Hugo is a popular static web site generator used for blogging. The posts are in markdown format.

Setup an environment, so that a non-technical user can edit a blog article (in markdown format)
online on github.com, and, when the user saves the file, it is published.

### Goal 1 - Walking Skeleton

Get everything running locally.

Setup system so that `hugo` doesn't have to be installed on the developer's system (developer system
== host system in this context). Use a docker container instead.

The only files on the host system should be the content of the blog: Markdown files.

- install `git`
- install `docker` (docker should be executable without needing `sudo` priviledges)
- find suitable docker "hugo" container, or create your own
- learn how to mount docker volumes to persist blog content
- (optional) git: organize docker configuration and blog content into separate repos

### Goal 2 - Start thinking, postpone decisions, but keep going

again: just some ideas:

- decide on deployment:
    - deploy docker container (needs more infrastructure...)
    - deploy static web sites (`public` folder from hugo)
- decide on ci strategy:
    - where is deployment trigger located? ci? git? github?
- security:
    - how important is it for the project?

### Goal 3 - automate

Make everything reproducable.

