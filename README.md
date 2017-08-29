# Java App Store Framework

NOTICE: This project was recently moved to its own repository. It was originally developed in the ‘Current’ repository (Now renamed to [UniCade](https://github.com/benlen10/UniCade)) which contains the previous commits and versions.  

# Project Description
- This project is a command line based app store that simulates the behavior of the Google Play store.

- The program was originally developed as a school project at UW Madison.  

# Getting Started
- Launch the AppStore program with the arguments specified below 
- java AppStore UserDataFile CategoryListFile AppDataFile AppActivityFile




# Supported operations



| l <email> <password>                     |    Logs in the user, if both email and password are valid. If an another user is already logged in, an error is displayed                                                                                                                      |
|------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| x                                        |  Logs out the current user, and starts the anonymous user mode                                                                                                                                                                                 |
| s                                        |    Subscribes a user as a developer, if not already. This should not work in anonymous mode.                                                                                                                                                   |
|    v categories                          |    View the list of all the categories, which a user can browse through.                                                                                                                                                                       |
|    v recent <category>                   | View the list of all apps,in the given category sorted by their upload timestamp.  If no category is,given, then display the list of all apps across all the categories. View the list of all the,categories, which a user can browse through. |
| v free <category>                        | View the list of all free apps in the given category sorted by the ranking score. If no category is specified, then display the list for all apps across all the categories.                                                                   |
| v app <appId>                            | View the details of an app specified through its app id.                                                                                                                                                                                       |
| d <appId>                                | Allows the user to download an app. If the user has already downloaded the app, display an error message. Does not work in anonymous mode.                                                                                                     |
| r <appId> <rating>                       |    Allows the user to rate an app. The rating should always be between 1-5. A user cannot the rate the   app, that he/she has not downloaded. Does not work in anonymous mode.                                                                 |
| u <app_name> <app_id> <category> <price> | Upload an app. Category is required. Price >= 0.0. One cannot upload an app name with a,duplicate app_id value. Does not work for non-developers.                                                                                              |
| p <email>                                |    Shows a user profile, with the given email.                                                                                                                                                                                                 |
| p                                        |    Shows the profile of the currently logged-in user. If the logged-in user is a developer, it will also show the total earnings made from all of his/her apps.                                                                                |
| q                                        |  Exits the application                                                                                                                                                                                                                         |