Creates a deep copy of the value which may contain (nested) `Array`s and
`Object`s, `Number`s, `String`s, `Boolean`s and `Date`s. `Function`s are
assigned by reference rather than copied

Dispatches to a `clone` method if present.

@func
@memberOf R
@since v0.1.0
@category Object
@sig {*} -> {*}
@param {*} value The object or array to clone
@return {*} A deeply cloned copy of `val`
@example

     var objects = [{}, {}, {}];
     var objectsClone = R.clone(objects);
     objects === objectsClone; //=> false
     objects[0] === objectsClone[0]; //=> false
