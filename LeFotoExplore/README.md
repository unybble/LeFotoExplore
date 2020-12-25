# Errors to look for

* Organization of folder structure is messy. Should separate out logical elements into separate folders
* App.vue should be a “base page” that calls the Day component and the Quote component. Should put components into their own folder.
* The services should implement an interface for the controller to call.
* The WeatherForecastService is not a Controller, and it should not be in that namespace.
* There should not be any logic in the controller. Put it into the service.
* There should be a separate folder for models. Do not put the QuoteResponse and Quote models in the same file as the Service file.
* Use a singleton for the HttpClient, it will improve performance
* Use Disposable anywhere it can be used, such as HttpResponse. Also improves performance.
* There are instances of doing the same call twice (DateTime). Should store in a variable and use later.
* While the Quote service is async, the controller calls it in a synchronous way. This can be blocking
* In the Day component, “list” is not a descriptive variable
* No inline styling in App.vue h1 tag
* Terrible CSS
* CSS has a magic number
* CSS has some non descriptive class names
* CSS are making a reference to the body style twice, which degrades performance
* The ordering of the classes and elements does not flow in a large —> small fashion.
* It would be better to import a css or sass file using an @import statement.
* The conditional statements for the icon should be in its own function
* The conditional statement method, as presented, is terrible
* Don’t do string comparisons (slow) plus if you are, ensure case does not play a role by having a ToLower() (note the bug)
* all of the IFs is not performant. Use if-else
* Use moment.js instead of doing weird things with the date string
* No comments
* Ugly implementation