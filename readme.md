# RequireJs-LiveJs

Just include Live.js and it will monitor the current page including local CSS and Javascript by sending consecutive HEAD requests to the server. Changes to CSS will be applied dynamically and HTML or Javascript changes will reload the page. Try it!



# Use

Add liveJs to your requirejs dependencies, then include a separate call to require in order to load liveJs last, something like:

    requirejs.config({
        baseUrl: '/src',
        paths:{
            livejs: '/bower_components/live/live'
        },
    });
    
    // Start the main app logic.
    requirejs([],
            function(){
                require(['livejs']);
            }
    );

This ensures that liveJs can see all the modules that requirejs has loaded. 

# Where?

Live.js works in Firefox, Chrome, Safari, Opera and IE6+ until proven otherwise. Live.js is independent of the development framework or language you use, whether it be Ruby, Handcraft, Python, Django, NET, Java, Php, Drupal, Joomla or what-have-you.

# History

Live.js was written by Martin Kool as the next step in Handcraft's design in the browser strategy. 
