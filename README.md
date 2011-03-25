Twitter profile widget internationalization
===================================

This is a fork of [Dustin Diaz](http://www.twitter.com/ded)'s original work on the [twitter profile widget](http://twitter.com/about/resources/widgets/widget_profile).

I only added the possibility to show the widget in any language (Klingon if you want...)

Instructions
------------

1. Download the forked js file named widget.js
2. Add it in your html/template file
3. Create your language dictionnary
4. Use the same old TWTR.widget
5. voilà!

Example usage
-------------
`
  TWTR.i18n.init({
    "join-the-conversation" : "Rejoignez la conversation"
    , "reply" : "Répondre"
    , "months" : [
      "Janvier", "Février", "Mars", "Avril", "Mai", "Juin", "Juillet"
      , "Août", "Septembre", "Octobre", "Novembre", "Décembre"
    ]
  , "right-now" : "maintenant"
  , "x-seconds-ago" : "Il y a %s secondes"
  , "about-1-minute-ago" : "Il y a environ 1 minute"
    , "x-minutes-ago" : "Il y a %s minutes"
    , "about-1-hour-ago" : "Il y a environ 1 heure"
    , "x-hours-ago" : "Il y a environ %s heures"
    , "yesterday" : "hier"
    , "x-days-ago" : "Il y a %s jours"
    , "over-a-year" : "Il y a plus d'un an"
  });

  new TWTR.widget({..}).render().setUser('twitter_user_name').start();
`

Known bugs
----------

* minified version doesn't work.