Angular UUID and GUID Generator
===========================

Angular UUID and GUID Generator

##How to use
###1
incluede `angular.uuid.js` or `angular.uuid.min.js` 
```html
<script src="angular.uuid.js"></script>
````

###2
---javascript
var app = angular.module('app',['angularUUID']);
-----

###3
Inject into your controller

---javascript
app.controller('mainCtrl', ['$scope','uuid', function($scope,uuid){

}])
----

###4.1
now you can get UUID 

---javascipt
app.controller('mainCtrl', ['$scope','uuid', function($scope,uuid){
	$scope.getId = function(){
		$scope.id = uuid.newuuid();
	}
}])
----
###4.2
or GUID 
---javascript
app.controller('mainCtrl', ['$scope','uuid', function($scope,uuid){
	$scope.getId = function(){
		$scope.id = uuid.newguid();
	}
}])
----

