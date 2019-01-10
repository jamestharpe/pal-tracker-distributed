# Pal Tracker Distributed

Follows the conventions set forth in the [App Continuum
Presentation](http://deck.appcontinuum.io/assets/player/KeynoteDHTMLPlayer.html).

In a nutshell:

**Start with MVC**: Models and Controllers.

**Convert to feature groups**: Defines the application's bounded contexts. Each feature contains the controllers, data 
access objects, and models required for the feature to function.

**Break feature groups into components**: Independently reusable groups of code (no circular dependencies between 
components). Each component can be built independently.

**Create separate applications using components**: Each application can be independently developed, tested, deployed, 
and scaled.


./gradlew cloudNativeDeveloperDistributedSystemDeployment \
    -PregistrationServerUrl=http://registration-pal-james-rupali.apps.evans.pal.pivotal.io \
    -PbacklogServerUrl=http://backlog-pal-james-rupali.apps.evans.pal.pivotal.io \
    -PallocationsServerUrl=http://tracker-allocations.apps.evans.pal.pivotal.io  \
    -PtimesheetsServerUrl=http://timesheets-pal-james-rupali.apps.evans.pal.pivotal.io
    
 