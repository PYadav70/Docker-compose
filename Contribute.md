## manual installation
- install node.js locally ()
- clone the repo
- install depedencies (npm install)
- start the DB locally ()
    - docker run -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres 
    -go to neon.tech and get yourself a new db
- change the .env file and update your DB credentials
- npx prisma migrate
- npx prisma generate
- npm run build
- npm run start


## DOCKER installation
-install docker
-start postgress
    - docker run -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres 
-Build the image - `Docker build --network=host -t user-project`
-start the image - `docker run -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres   -p 3000:3000 user-project`


## DOCKER COMPOSE INSTALLATION STEPS
-install docker
-docker compose
-Run `docker-compose up`
