# ANGULAR 12

## 1.  Install Angular 
    
     npm install -g @angular/cli    ((install Angular))

## 2. Check version

     ng --version  ((check version))  

## 3. Create Angular Boilerplate 
     ng new "file name"        ((does complete file setup and all files needed for you))
    
    ----> do this in your root directory as it will create a root project folder for you

## 4. get app running 

    ng serve ((starts app))

## 5. create components
    
    ng g component components/"component name" - creates new component and file structure

## API calls in Angular 

### make a service

    ng g service "service name"

    - generates two files 
        - src/app/"service name".service.spec.ts
        - src/app/"service name".service.ts

### update app.modules.ts 

    import {HttpClientModule} from '@angular/common/http'

    also dont forget to add HttpClientModule to Imports: (within @ngModule)

### update "service name".service.ts

    import {HttpClient} from '@angular/common/http'

    within constructor:

    constructor(private http: HttpClient) { }