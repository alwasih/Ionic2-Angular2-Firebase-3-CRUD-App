# Ionic2-Angular2-Firebase-3-CRUD-App
A working Ionic2/Angular2/AngularFire2/Firebase3 CRUD app anyone can clone

Some Initializations:

Firebase Databases, by default are setup to only be accessible while authenticated. So in order to have this project work properly, the firebase database needs to have those restrictions taken off.

So once you create the firebase storage app on your firebase.google.com console, you will need to go into the "Rules" section (Click "Database" on the left pane, and then select the "Rules" tab on the right) and change the default rules. Delete everything there and insert this instead:

{
    "rules": {    
        ".read": true,
        ".write": true
    }
}

Keep in mind that once you have a public app, you will need to change this back to prevent anyone and everyone adding data to your database.
