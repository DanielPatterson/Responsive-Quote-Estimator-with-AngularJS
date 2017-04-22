# Responsive-Quote-Estimator-with-AngularJS
Responsive Quote Estimator with AngularJS

#### controller.js

```js
function OrderFormController($scope){

	$scope.items = [
		{
			name: 'Social Media Campaign',
			desc: 'loreum ipsum dolar sit amet',
			price: 8000, // to change price change this number
			active: false
		},
		{
			name: 'Search Engine Optimsiation',
			desc: 'loreum ipsum dolar sit amet',
			price: 10000, // to change price change this number
			active: false
		},
		{
			name: 'CMS Intergration',
			desc: 'loreum ipsum dolar sit amet',
			price: 15000, // to change price change this number
			active: false
		},
		{
			name: 'User Testing',
			desc: 'loreum ipsum dolar sit amet',
			price: 20000, // to change price change this number
			active: false
		},
		{
			name: 'Accessibility Audit',
			desc: 'loreum ipsum dolar sit amet',
			price: 25000, // to change price change this number
			active: false
		},
		{
			name: 'Usability Audit',
			desc: 'loreum ipsum dolar sit amet',
			price: 30000, // to change price change this number
			active: false
		},
		{
			name: 'Design',
			desc: 'loreum ipsum dolar sit amet',
			price: 40000, // to change price change this number
			active: false
		},
		{
			name: 'Development',
			desc: 'loreum ipsum dolar sit amet',
			price: 60000, // to change price change this number
			active: false
		}
		 
	];
	

	$scope.toggleActive = function(s){
		s.active = !s.active;
	};

	$scope.total = function(){

		var total = 0;

		angular.forEach($scope.items, function(s){
			if (s.active){
				total+= s.price;
			}
		});
		
		return total;
	};

	
}
```
