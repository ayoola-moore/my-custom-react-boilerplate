** Project name**

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app) ...

- Project requirement can be found here-

- Project dependency include puppeteer, axios, and style-compoonent. Reference package.json for complete list.

**System configuration used**

> node js v10.19.0
> Does not support WSL because of chromium used

**Build and Production**

```
    npm install
    npm run build
    npx serve -g build
```

**Development and Testing**

```
    npm install
    npm run start
    npm run test
```

**Project Structure (modularity design)**

The architectural pattern used was adopted with scalability in mind and tries to adopt the domain driven design

- src/utils :
  Should contain shared assets designed to be used across the entire application eg. css reset, common functions etc.
- src/components
  Should contain react components designed to be reusable and shared across the application
- src/{featureName}

  - Each identifiable feature will contain its own directory eg. displayFeeds
  - The directory is aimed at following an easily adoptable and repeatable pattern based on functionalities. ( I will be happy to shade more light of the choice of architectural pattern adopted if need be)

- page: for routing based pages.
- Files and directories were all named using camelCased
