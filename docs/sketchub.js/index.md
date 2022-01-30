# Sketchub.js

An easier way to use Sketchub's api in JavaScript or TypeScript.

## Getting Started

### Installation

- With NPM: 
  `npm i sketchub.js`
- With Yarn: 
  `yarn add sketchub.js`

### Adding Sketchub.js

```js
const { Sketchub } = require('sketchub.js');
const apiClient = new Sketchub();

apiClient.setApiKey(process.env.API_KEY);
```

### Making api calls

```js
apiClient.getCategories((response) => {
  console.log(response);
});

apiClient.getProjectDetails('1', (response) => {
  console.log(response);
});

apiClient.getProjectList('1', (response) => {
  console.log(response);
});
```
