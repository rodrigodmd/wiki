
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

# Let's get to work

Now you can start using the components:

- https://valor-software.com/ngx-bootstrap/#/accordion
- https://getbootstrap.com/docs/4.1/components/alerts/

To use a module, first you need to add it in the app module.
For example to use the dropdown, open src/app/app.module.ts and add:

```typescript
import { BsDropdownModule } from 'ngx-bootstrap/dropdown';
...

@NgModule({
   ...
   imports: [BsDropdownModule.forRoot(), ... ],
    ...
})
```

Now you can work in the HTML.
open src/app/app.component.html and add:
```typescript 
<div class="btn-group" dropdown>
  <button dropdownToggle type="button" class="btn btn-primary dropdown-toggle">
    Button dropdown <span class="caret"></span>
  </button>
  <ul *dropdownMenu class="dropdown-menu" role="menu">
    <li role="menuitem"><a class="dropdown-item" href="#">Action</a></li>
    <li role="menuitem"><a class="dropdown-item" href="#">Another action</a></li>
    <li role="menuitem"><a class="dropdown-item" href="#">Something else here</a></li>
    <li class="divider dropdown-divider"></li>
    <li role="menuitem"><a class="dropdown-item" href="#">Separated link</a>
    </li>
  </ul>
</div>
```
Run the app in demo mode and ensure the dropdown button functions correctly.