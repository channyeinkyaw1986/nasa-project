# NASA Mission Control Project

The completed version of our NASA project from [Complete Node.js Developer: Zero to Mastery](https://academy.zerotomastery.io/p/learn-node-js?affcode=441520_1jw4f2ay).

Keep in mind that we recommend you code along with us and use this only if you ever get stuck or you don't like to code along.

## Getting Started

1. Ensure you have Node.js installed.
2. Create a free [Mongo Atlas](https://www.mongodb.com/atlas/database) database online or start a local MongoDB database.
3. Create a `server/.env` file with a `MONGO_URL` property set to your MongoDB connection string.
4. In the terminal, run: `npm install`

## Running the Project

1. In the terminal, run: `npm run deploy`
2. Browse to the mission control frontend at [localhost:8000](http://localhost:8000) and schedule an interstellar launch!

## Docker

1. Ensure you have the latest version of Docker installed
2. Run `docker build . -t username/nasa-project`
3. Run `docker push username/nasa-project`
4. Run `docker run -it -p 8000:8000 username/nasa-project`

## Running the Tests

To run any automated tests, run `npm test`. This will:

* Run all the client-side tests: `npm test --prefix client`
* Run all the server-side tests: `npm test --prefix server`

## Running Docker on AWS

* [Docker basics for Amazon ECS](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/docker-basics.html)

1. Run `sudo yum update -y`
2. Run `sudo yum install docker`
3. Run `sudo service docker start`
4. Run `sudo usermod -a -G docker ec2-user`
5. Run `docker info`
6. Run `docker run --restart=always -p 8000:8000 username/nasa-project`

## Nodejs Security

* [NodeJS Security Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Nodejs_Security_Cheat_Sheet.html)
