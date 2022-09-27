<div align="center" style="margin-bottom: 20px;">
  <h1>SERVER (API)</h1>
  <p align="center">
    <img alt="technology" src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white">
    <img alt="technology" src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white">
    <img alt="technology" src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white">
    <img alt="technology" src="https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=Prisma&logoColor=white">
    <img alt="technology" src="https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white">
  </p>
</div>


### About project
API of our esports-duo project, at the base of its development we used typescript, node.js and the express.js framework, this api is responsible for reading and writing data in a SQL database, for this project we used the SQLite but it is possible to change and use another database.


#### Main technologies
- [TypeScript](https://www.typescriptlang.org/docs/)
- [Node.js](https://nodejs.org/en/)
- [Express.js](https://expressjs.com/)
- [Prisma](https://www.prisma.io/docs/getting-started)
- [SQLite](https://www.sqlite.org/index.html)


#### Run this project
```bash
# clone this project
$ git clone https://github.com/jefferson1104/esports-duo.git

# access the project folder
$ cd esports-duo/server

# install dependencies
$ npm install

# run sqlite database migration
$ npx prisma migrate dev

# run prisma client to open sqlite database
$ npx prisma studio

# run the project on the local machine
$ npm run dev
```

#### Endpoints
**Create game** - `POST` /games/{game_id}/ads</br>
**List ads by game** - `GET` /games/{game_id}/ads</br>
**Get discord by ad** - `GET` /ads/{ad_id}/discord</br>
**List games** - `GET` /games
