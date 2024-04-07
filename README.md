# angular-monorepo-microfrontend
Angular Monorepo Microfrontend

# Commands
ng new monorepo-workspace --create-application=false
cd monorepo-workspace
ng g application shell-app --routing --style=scss
ng g application auth-app --routing --style=scss
ng g application feature-one-app --routing --style=scss
ng add @angular-architects/module-federation --project shell-app --port 4200
ng add @angular-architects/module-federation --project auth-app --port 4300
ng add @angular-architects/module-federation --project feature-one-app --port 4400
ng s shell-app -o
ng s auth-app -o
ng s feature-one-app -o
