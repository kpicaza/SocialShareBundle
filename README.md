This bundle is based on work of  Gregquat from http://obtao.com/blog/2012/11/social-buttons-bar-for-facebook-twitter-google-with-symfony/

Instalation:

Add to project composer.json
    
        "require": {
            ...
            "stfalcon/tinymce-bundle": "dev-master",
            ...
        }


Usage:
    
    // insert the whole bar with default values
    {{ socialButtons() }}

    // insert the Twitter button only
    {{ twitterButton() }}
    // or 
    {{ socialButtons( {'googleplus':false, 'facebook':false} ) }}

    // insert the google+ button with custom parameters
    {{ googlePlusButton( {'locale':'fr', 'url':'http://google.fr' }) }}

    // insert the bar with specific values for Facebook
    {{ socialButtons( { 'facebook': {'locale':'fr_FR', 'send':true}} ) }}