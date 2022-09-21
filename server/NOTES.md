### INSTALL TYPESCRIPT
```bash
# install typescript
$ npm install -D typescript

# install ts-node-dev
npm install -D ts-node-dev

# create tsconfig.json
$ npx tsc --init
```

In the **package.json** file in the scripts section we will create as in the example below:
```json
  "scripts": {
    "build": "tsc",
    "dev": "tsnd src/server.ts"
  }
```

Agora no arquivo **tsconfig.json** faça algumas alterações: 
- Troque `// "module": "commonjs",` por `"module": "CommonJS",`
- Troque `// "rootDir": "./",` por `"rootDir": "./src",`
- Troque `// "outDir": "./",` por `"outDir": "./build",`
- Troque `// "moduleResolution": "node",` por `"moduleResolution": "node"`,

### INSTALL PRISMA
```bash
# install prisma
$ npm install -D prisma

# Init prisma using sqlite provider in this example
$ npx prisma init --datasource-provider SQLite

# Create migration
$ npx prisma migrate NAME_MIGRATION

# Navigate in your database
$ npx prisma studio
```


### PROJECT
```bash
# start api
$ npm run dev

# build api
$ npm run build
```