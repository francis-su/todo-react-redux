
# important concepts

 1. action
 2. reducer
 3. store
 4. middleware
 5. presentational/container component

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

# questions

 1. Is it reasonable that `component` and `container` contains each other? e.g. `Footer` contains `FilterLink`, while `VisibleTodoList` contains `TodoList`.
 2. how to design state tree
 3. how to design component hierarchy
 	* design presentational component
 	* design container component
 	* design other component