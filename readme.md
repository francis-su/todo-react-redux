
# blunders / pitfalls
	1. forgot to export component class when defines component
	2. incorrectly using arrow function result in the `state` being updated unexpectedly, for example
	```
		[1,2,3].map(item => item * 2);
	```
	
	vs

	```
		[1,2,3].map(item => {
			item * 2;
		});
	```

