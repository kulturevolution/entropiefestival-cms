# entropiefestival CMS

This is the repository for the entropiefestival CMS. It is based on the [Strapi](https://strapi.io/) headless CMS.

## Development
To start strapi locally, create a `.env` file in the root directory with the following content:
```
HOST=0.0.0.0
PORT=1337
APP_KEYS=key1,key2,key3,key4
API_TOKEN_SALT=salt
ADMIN_JWT_SECRET=secret
TRANSFER_TOKEN_SALT=salt
# Database
DATABASE_CLIENT=postgres
DATABASE_HOST=dbhost
DATABASE_PORT=dbport
DATABASE_NAME=dbname
DATABASE_USERNAME=dbuser
DATABASE_PASSWORD=dbpassword
DATABASE_SSL=false
JWT_SECRET=secret
```
Then run:
```
yarn install
yarn develop
```
## Live Deployment
When pushing to the `main` branch, a new package will be built with the tag `latest`.   
Run `docker compose up -d` on the live server to deploy the new version.
