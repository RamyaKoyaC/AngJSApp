# AngJSApp

## Used to Type in a Name and display as full name! 
<html>
   
   <head>
      <title>Angular JS Controller</title>
      <script src = "https://ajax.googleapis.com/ajax/libs/angularjs/1.3.14/angular.min.js"></script>
   </head>
   
   <body>
      <h2>Enter your name </h2>
      
      <div ng-app = "App1" ng-controller = "studentController">
         Enter first name: <input type = "text" ng-model = "student.firstName"><br><br>
         Enter last name: <input type = "text" ng-model = "student.lastName"><br>
         <br>
         
         Hi {{student.fullName()}}! 
      </div>
      
      <script>
         var App1 = angular.module("App1", []);
         
         App1.controller('studentController', function($scope) {
            $scope.student = {
               firstName: "",
               lastName: "",
               
               fullName: function() {
                  var studentFullName;
                  studentFullName = $scope.student;
                  return " " + studentFullName.firstName + " " + studentFullName.lastName;
               }
            };
         });
      </script>
      
   </body>
</html>



## Second program is to use filters in AngJS:

