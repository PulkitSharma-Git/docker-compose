## Manual Installation
- Install nodejs locally
- Clone the repo
- Install depencdencies
- Start DB (get your postgres db string)
- Create the env file and put your db creds POSTGRES_URL = 
- npx prisma migrate dev
- npx prisma generate
- npm run build
- npm run start

## Docker Installation

- Install Docker
- Create a network - docker network create user_project
- Start postgres
    - docker run --network user_project --name postgres -e POSTGRES_PASSWORD=TINNA -d -p 5432:5432 postgres   
- Build the Image - "docker build --network=host -t user-project ."
- Start the Image - "docker run -e DATABASE_URL=postgresql://postgres:TINNA@postgres:5432/postgres --network user_project -p 3000:3000 user-project 

## Docker compose Installation
- Install docker, docker- compose
- Run 'docker-compose up

