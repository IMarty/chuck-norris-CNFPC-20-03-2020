https://github.com/IMarty/chuck-norris-CNFPC-20-03-2020

# Process

0. Check the API
  you are making the good request to the good endpoint
  https://languagelayer.com/php_helper_scripts/language_api.php?secret_key=0d1227d3c54c395bcc7bf80a5927fde9&query=Hello


1. Service
Create the right function inside the service
 - We need to app the httpclientModule to the app.module.ts
 - We need the load the httpclient as a private ressource

2. Component
ng g c components/page-joke

3. Create the routing in app-routing.module

  {
    path: '',
    redirectTo: 'joke',
    pathMatch: 'full'
  },
  {
    path: 'joke',
    component: PageJokesComponent
  }

4. Load the data in the component TS with the use of the service and the subscibe

5. Show the data in the component HTML .. don't forget to use the directives
    Library for the flags : flag-icon-css
    Use the "language_code"


# Continuous Intergration
Create a Github Repository linked to your project
Go to "netlify.com" to create a "new site from git"
In the deploy section :
- command : ng build --prod
- folder : dist/chuck-norris

# Progressive Web Application
Allow offline Access, but not do the get request of course
and allow the use to install the application on his device.

ng add @angular/pwa in your working folder

# Enable the routing on all pages
https://stackoverflow.com/questions/51887581/angular-routing-not-working-on-netlify-on-page-refresh


