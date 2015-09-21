Emerald CI
==========

Emerald CI want to pursue a Docker Compose driven development. You test your
software on the CI server just like you test locally, it drastically reduces
the risk of breaking the build due to differences of the environments. It uses
the same `docker-compose.yml` specification as Docker Compose, therefore all
you need is a `docker-compose.yml` and a minimal config in your repo.

Setup your own
--------------

Since Emerald CI wants to pursue a Docker Compose driven development, deploying
it is a matter of a `docker-compose.yml`. You can use your favorite
orchestration tools which support the compose specification.

> We like to use [Rancher](http://rancher.com/) and
> [rancher-compose](https://github.com/rancher/rancher-compose). Using
> rancher-compose it is just a matter of `rancher-compose up` to setup the
> whole system.

An example
[`docker-compose.yml`](https://github.com/emerald-ci/Emerald-CI/blob/master/docker-compose.yml)
has been placed in this repo to deploy the system. Take it, deploy, test and
have fun! :smile:

> Please make sure to change environment variables to match your setup and
> change secrets!

What's to come
--------------

Right now Emerald CI only tests your software. To complete the Continuous
Development cycle, deployment has to be added. The plan is to allow writing
plugins as docker images which get the build context passed.

Issues
------

This is a meta repo. Report all issues for
[here](https://github.com/emerald-ci/Emerald-CI/issues).
