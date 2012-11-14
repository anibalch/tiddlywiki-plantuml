tiddlywiki-plantuml
===================

Description
-----------
Plugin for easy integration of UML diagrams in [TiddlyWiki](http://tiddlywiki.com), using [PlantUML](http://plantuml.sourceforge.net).

The diagrams are written inside Tiddlywiki tiddlers, using the PlantUML syntax, and will be shown as images when the tiddler is opened.

It only works online, as it uses the online [PlantUML server](http://www.plantuml.com) to generate the images.

Installation
------------
To include the plugin in your TiddlyWiki, create a tiddler for it: new tiddler, with the plugin code (`PlantUmlPlugin.js`) as the content, and with a tag called `systemConfig`.

Usage
-----
To use it, you'll have to use the macro `plantUml` in your tiddler, with the following format: 

    <<plantUml 'diagram specification' 'alternate text'>>

Where the `'alternate text'` is optional.

Example:

    <<plantUml
    '@startuml
    Alice -> Bob: Authentication Request
    Bob --> Alice: Authentication Response
    @enduml'
    'simple sequence diagram'
    >>

Author
------
Feel free to address your comments/suggestions/whatever to yours truly:

    Aníbal Cáceres
    anibal.caceres@gmail.com

