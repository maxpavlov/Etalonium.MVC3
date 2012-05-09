Etalonium.MVC3
==============

This is a template ASP.NET MVC 3 Visual Studio solution that is Html5 Boilerplate-enabled, has a custom Razor-based view engine that supports localized views and has a [client dependency framework](http://clientdependency.codeplex.com/) set up. 

So when you need a localized version of a view, let's say, an Index view, you just create a `Index.**fr**.cshtml` localized view and add language specific contents to it. (**fr** is for french, just for examples' sake. This can be any language two letter code).

Also language change support via cookies is provided. And via query string parameter "lang". So if you want to trigger chinese view, you just add this to your request string:

`localhost:4545/?lang=ch`

and the `Index.ch.cshtml` will render out into the browser(given that in is routed to by default of course)

Look into global.cs to see how to set the current language from javascript code.

The default browser locale will set the current culture and language automatically thanks to 

`<globalization enableClientBasedCulture="true" culture="auto" uiCulture="auto"/>`

in web.config.