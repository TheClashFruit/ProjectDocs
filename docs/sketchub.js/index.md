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

apiClient.getProjectTypes((response) => {
  console.log(response);
});

apiClient.getProjectDetails(1, (response) => {
  console.log(response);
});

apiClient.getProjectList(1, (response) => {
  console.log(response);
});

apiClient.findUserName('Amitoj', (response) => {
  console.log(response);
});

apiClient.getUser('412', (response) => {
  console.log(response);
});

apiClient.getAnnouncements((response) => {
  console.log(response);
});

apiClient.getMeta((response) => {
  console.log(response);
});

// OR

const getProjectTypes   = await apiClient.getProjectTypes();
const getProjectDetails = await apiClient.getProjectDetails(1);
const getProjectList    = await apiClient.getProjectList(1);
const findUserName      = await apiClient.findUserName('Amitoj');
const getUser           = await apiClient.getUser('412');
const getAnnouncements  = await apiClient.getAnnouncements();
const getMeta           = await apiClient.getMeta();

console.log(getProjectTypes);
console.log(getProjectDetails);
console.log(getProjectList);
console.log(findUserName);
console.log(getUser);
console.log(getAnnouncements);
console.log(getMeta);
```
