# ember-cli-deploy-datadog-asset-sizes

[WIP]

Keep track of your ember apps asset sizes over time. Each deploy the addon will push your apps assets sizes to DataDog.

## Installation

```sh
ember install ember-cli-deploy-datadog-asset-sizes
```

### Add you DataDog keys
Add your DataDog key to deploy.js

```js
module.exports = function(deployTarget) {
  var ENV = {
    // truncated for brevity
    emberCliDeployAssetSizes: {
      DATADOG_API_KEY: <your-api-key>,
      DATADOG_APP_KEY: <your-app-key>,
      DATADOG_NAMESPACE: <some-namespace>
    }
  };

  // truncated for brevity
  return ENV;
};
```
## Deploy

```sh
ember deploy production
```

## Running Tests

* `npm test` Comming soon! :(


For more information on using ember-cli-deploy, visit [ember-cli-deploy.com](http://ember-cli-deploy.com/).
