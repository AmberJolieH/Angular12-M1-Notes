# ANGULAR 12

## 1.  Install Angular 
    
     npm install -g @angular/cli    ((install Angular))

## 2. Check version

     ng --version  ((check version))  

## 3. Create Angular Boilerplate 
     ng new "file name"        ((does complete file setup and all files needed for you))
    
    ----> do this in your root directory as it will create a root project folder for you
    
    - app.component.css file contains the style sheets of the main app component. Styles can be defined locally for each component
   
    - app.component.html contains the HTML template of the component
    
    - app.component.ts file contains the code controlling the view
    
    - app.module.ts defines which modules your app will use
    
    - app-routing.module.ts is set up to define the routes for your application
   
    - app.component.spec.ts contains a skeleton for unit testing the app component

## 4. get app running 

    ng serve ((starts app))

## 5. create components
    
    ng g c componentName - creates new component and file structure

## 6.  API calls in Angular 

###  * make a service

    ng g service "service name"

    - generates two files 
        - src/app/"service name".service.spec.ts
        - src/app/"service name".service.ts

### * update app.modules.ts 

    import {HttpClientModule} from '@angular/common/http'

    also dont forget to add HttpClientModule to Imports: (within @ngModule)

### * update "service name".service.ts

    import {HttpClient} from '@angular/common/http'

    within constructor:

    constructor(private http: HttpClient) { }