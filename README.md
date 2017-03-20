# Simple Angular2 Service

A service for using localstorage in angular2 apps that returns observables.

That simple.

## Install:

```npm install ng2-localstorage -S```

## Implementation

In your app.module you simply need to import the configuration options and module from
the module, and then pass it to your module. The configuration is optional, and will
have a defualt storage prefix of 'ngl'

```
import { NG2LocalStorageModule, NG2LocalStorageConfig } from 'ng2-localstorage';

export const myLocalStorageModules: NG2LocalStorageConfig = {
  prefix: 'myPrefix',
  storageType: 'local'
};

@NgModule({
  imports: [
    NG2LocalStorageModule.forRoot(myLocalStorageModules)
  ]
})
```

