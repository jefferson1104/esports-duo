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
