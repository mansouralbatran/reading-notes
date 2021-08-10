# Lists and Keys


![image](https://i.morioh.com/200626/ec9a9e94.jpg)
1.  Rendering Multiple Components
   * You can build collections of elements and include them in JSX using curly braces {}


2.  Basic List Component
 * Usually you would render lists inside a component.

We can refactor the previous example into a component that accepts an array of numbers and outputs a list of elements.
    
3.  Keys
 * Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:


4.  Extracting Components with Keys

  * Keys only make sense in the context of the surrounding array.


5.  Keys Must Only Be Unique Among Siblings

  * Keys used within arrays should be unique among their siblings. However, they don’t need to be globally unique. We can use the same keys when we produce two different arrays:

