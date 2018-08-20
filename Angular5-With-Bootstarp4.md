## INSTALLING ANGULAR CLI
    npm install -g @angular/cli

## CREATE A NEW APPLICATION

    ng new eventmanager --style=scss
    cd eventmanager
    ng serve

## ADD BOOTSTRAP & BOOTSWATCH

    npm install --save bootstrap
    npm install --save bootswatch

import bootwatch and bootstarp
    src/styles.scss

    @import "~bootswatch/dist/yeti/_variables.scss";
    @import "~bootstrap/scss/bootstrap.scss";
    @import "~bootswatch/dist/yeti/_bootswatch.scss";

## ADDING FONT-AWESOME
    npm install --save font-awesome

    .angular-cli.json
    {
      "apps": {
        "styles": [
          "styles.scss",
          "../node_modules/font-awesome/scss/font-awesome.scss"
        ],
        "addons": [
          "../node_modules/font-awesome/fonts/*.+(otf|eot|svg|ttf|woff|woff2)"
        ]
      }
    }
## CREATE MAIN PAGE CONTENT
## test bootstarp
```
/src/app/app.component.html
<div class="container" style="margin-top: 10px;">
  <router-outlet></router-outlet>
</div>
```