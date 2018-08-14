
# [ngx-bootstrap](https://valor-software.com/ngx-bootstrap/#/)

ngx-bootstrap contains all core (and not only) Bootstrap components powered by Angular. So you don't need to include original JS components, but we are using markup and css provided by Bootstrap.


# [Installation instructions](https://valor-software.com/ngx-bootstrap/#/getting-started):

Install bootrsap style:

    npm install bootstrap --save

Add bootstrap style in global style.scss:
```scss
@import '~bootstrap/scss/bootstrap.scss'
````
Install ngx-bootstrap from npm:

    npm install ngx-bootstrap --save


Sometimes, your project might contain some library that could interfear with the bootstrap framework, or you might have a customized version of bootstrap. The consequence is that the process of determining bootstrap version might be failed, which can break the UI. In that case, we can still set the bootstrap version manually in the boostraping component (i.e. AppComonent):

```typescript
import { setTheme } from 'ngx-bootstrap/utils';
 
@Component({…})
export class AppComponent {
  constructor() {
    setTheme('bs4'); // or 'bs3'
    …
  }
}
```