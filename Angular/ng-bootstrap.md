# Angular Boostrap widgets

Angular widgets built from the ground up using only Bootstrap 4 CSS with APIs designed for the Angular ecosystem.

No dependencies on 3rd party JavaScript.


Home: https://ng-bootstrap.github.io/#/home


# [Getting started](https://ng-bootstrap.github.io/#/getting-started)

Install ng-bootstrap via npm:

    npm install --save @ng-bootstrap/ng-bootstrap

Once installed you need to import our main module.

```typescript
import {NgbModule} from '@ng-bootstrap/ng-bootstrap';

@NgModule({
    ...
    imports: [NgbModule, ...],
    ...
})
export class YourAppModule {
}
```
Alternatively you could only import modules with components you need, ex. pagination and alert. The resulting bundle will be smaller in this case.

```typescript
import {NgbPaginationModule, NgbAlertModule} from '@ng-bootstrap/ng-bootstrap';

@NgModule({
  ...
  imports: [NgbPaginationModule, NgbAlertModule, ...],
  ...
})
export class YourAppModule {
}
```

## SystemJS
If you are using SystemJS, you should also adjust your configuration to point to the UMD bundle.

In your systemjs config file, map needs to tell the System loader where to look for ng-bootstrap:

```typescript
map: {
  '@ng-bootstrap/ng-bootstrap': 'node_modules/@ng-bootstrap/ng-bootstrap/bundles/ng-bootstrap.js',
}
```



Info about components: https://ng-bootstrap.github.io/#/components/accordion/examples