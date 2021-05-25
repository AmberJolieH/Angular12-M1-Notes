# ANGULAR 12

1. npm install -g @angular/cli    ((install Angular))

2. ng --version  ((check version))  // do this in your root directory as it will create a root project folder for you

3. ng new "file name"        ((does complete file setup and all files needed for you))

4. ng serve ((starts app))

5. ng g component components/"component name" - creates new component and file structure



# API calls in Angular 

## make a service

    ng g service "service name"

    - generates two files 
        - src/app/"service name".service.spec.ts
        - src/app/"service name".service.ts

## update app.modules.ts 

    import {HttpClientModule} from '@angular/common/http'

    also dont forget to add HttpClientModule to Imports: (within @ngModule)