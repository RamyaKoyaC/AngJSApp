# AngJSApp

<html>
   
   <head>
      <title>AngularJS First Application</title>
   </head>
   
   <body>
      <h1>First Application</h1>
      
      <div ng-app = "">
         <p>First Name <input type = "text" ng-model = "firstname"></p>
         <p>Last Name <input type = "text" ng-model = "lastname"></p>
         <p>Hello <span ng-bind = "firstname + lastname" ></span>!</p>
      </div>
      
      <script src = "https://ajax.googleapis.com/ajax/libs/angularjs/1.3.14/angular.min.js">
      </script>
      
   </body>
</html>
