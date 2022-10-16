# edu-auth-js

> The project creates a node.js backen application with express.
> It is set up with jest, and configured to run jest with jest-runner-groups.

## Application & Development

```bash
cd ~
cd ws
mkdir edu-auth-js
cd du-auth-js
npm init -y
npm pkg set main="app.js"
npm pkg set description="Simple application to test jwt"
npm pkg set scripts.start="node app.js" 
npm pkg set scripts.dev="nodemon app.js"

npm install express
npm install dotenv

npm install nodemon -D

curl -L  https://gist.github.com/miwashiab/da85ca45cff611f9e789a07577c348d5/raw/app.js -o app.js
curl -L  https://gist.github.com/miwashiab/b0c0569b2a4f0427c3374789a7aab52b/raw/server.js -o server.js
curl -L https://gist.github.com/miwashiab/3378fc2e4ab5d2691fa5978822721796/raw/.gitignore -o .gitignore

```

## Testing
```
mkdir __tests__
npm pkg set scripts.test="jest  --group=-component --group=-integration"
npm pkg set scripts.componenttest="jest  --group=component"
npm pkg set scripts.integrationtest="jest  --group=integration"

npm install jest -D
npm install jest-runner-groups -D
npm install supertest -D

curl -L https://gist.github.com/miwashiab/b3dd55fba37616c0d3820a06f0339eb9/raw/jest.config.js -o jest.config.js

curl -L https://gist.github.com/miwashiab/b127c7a83f4eef979a8935bbae3f9fe7/raw/unit_test.js -o ./__tests__/unit_test.js
curl -L https://gist.github.com/miwashiab/3960996c3bfca2e9b81189c884f74b75/raw/component_test.js -o ./__tests__/component_test.js
curl -L https://gist.github.com/miwashiab/8d39beda3493d4e5c6b46c2a5f94efc3/raw/integration_test.js -o ./__tests__/integration_test.js
```


## Healthcheck

```bash
npm install health-check
```
