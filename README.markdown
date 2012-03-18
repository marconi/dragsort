This is a github mirror of jQuery List DragSort (http://dragsort.codeplex.com) with a slight modification to allow underscorejs' _.binAll to work as usual with backbonejs.

ie:

    SomeView = Backbone.View.extend({
      initialize: function() {
        _.bindAll(this, 'someMethod')

        ...
      },
      someMethod: function(item) {
        ...
        // this => SomeView
        // item => itemSelector
      }
    })

