# Said Kholov - 7 April
## Installation

### Docker

https://docs.docker.com/install/

### Docker Compose

https://docs.docker.com/compose/install/

## Launch the app

`docker-compose -f docker-compose.dev.yml up`

## Features
<!-- Any special features / interesting details with your implementation you want to explicitly
note -->
## Security
* Only officially supported docker images used
* `npm audit fix` was run and all dependencies updated
* jest has minor security issue in one its dependencies.
This can be fixed by ejecting the create-react-app and upgrading jest manually.

## Improvements

1. Coverage review app can be improved in several ways. For example, It can be hosted in separate docker container or served as a static file from AWS S3.
2. Coverage could somehow be added to gitlab-route map. Unfortunately, I didn't have time to figure it out.
3. It would be better to have default `docker-compose.yml` for local development and have another file for deployment purposes. It would make running local instance simpler
4. Add production build
5. Eject react app; the app is only for test, so I didn't do it
    - customize lint configs for the dev team
    - update necessary packages
    - set up test coverage threshold
    - set up precommit hooks
