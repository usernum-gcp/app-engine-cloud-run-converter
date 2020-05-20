# App Engine to Cloud Run

Helper tool to migrate an App Engine service to a Cloud Run service.

Data is never uploaded. All processing is happening client side.  

This is not an officially supported Google product.

## How to use

### User interface

* Open index.html or [click here](https://googlecloudplatform.github.io/app-engine-cloud-run-converter/)
* Copy paste your `app.yaml`
* Enter other information (project ID, region...)
* Get your Cloud Run configuration file and deployment commands. 

### Programatically

Load the `app-to-run.js` module in your codebase with: 

```
import { appToRun } from './app-to-run.js';
```

Then invoke `appToRun()` with an option containing the App Engine configuration. See [this example](https://github.com/GoogleCloudPlatform/app-engine-cloud-run-converter/blob/master/index.js#L28)

TODO: document the exact API when it is stable.