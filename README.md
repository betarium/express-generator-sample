[install]

```
pnpx express --no-view --git express-generator-sample
cd express-generator-sample

git init
git add .
git commit -m "init project"

pnpm install typescript
pnpx tsc --init
pnpm install ejs
pnpm install -D @types/node
pnpm install -D @types/express
pnpm install -D ts-node
pnpm install -D ts-node-dev

pnpm install

git add .
git commit -m "support typescript"

mkdir src
move routes\index.js src\top.ts
move routes\users.js src\users.ts
move app.js src\app.ts
move bin\www src\index.ts

rmdir bin
rmdir routes

git add .
git commit -m "move source"
```
