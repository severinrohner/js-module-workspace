#Use of Bricks 
##In JS
```javascript
    // Workaround because it's undefined, fixed with Liferay 7 GA4 
    // https://web.liferay.com/de/community/forums/-/message_boards/view_message/86256824
    Liferay.Loader = Loader;  
    
    require('dep-bricks/Bricks.es', function(BricksModule) {
     var Bricks = BricksModule.default();
     console.log(Bricks);
     // Use of Bricks 
     // https://github.com/callmecavs/bricks.js
     
    }, function(error) {
        console.error(error);
    });
```

##In JSP

<aui:script require="dep-bricks/Bricks.es">
    Bricks = depBricksBricksEs.default;
</aui:script>
