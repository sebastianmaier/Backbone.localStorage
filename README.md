## Added: If no localStorage property is defined on the model or collection, the original Backbone.sync will be used

# Backbone localStorage Adapter v1.0

Quite simply a localStorage adapter for Backbone. It's a drop-in replacement for Backbone.Sync() to handle saving to a localStorage database.

## Usage

Include Backbone.localStorage after having included Backbone.js:

    <script type="text/javascript" src="backbone.js"></script>
    <script type="text/javascript" src="backbone.localStorage.js"></script>

Create your collections like so:

    window.SomeCollection = Backbone.Collection.extend({
      
      localStorage: new Store("SomeCollection"), // Unique name within your app.
      
      // ... everything else is normal.
      
    });
  
Feel free to use Backbone as you usually would, this is a drop-in replacement.

## Credits

Thanks to [Mark Woodall](https://github.com/llad) for the QUnit tests.