# If you need some extra help with the `Adapter` on this assignment...
What we're looking to achieve for the `Adapter` is relatively minimal: You might remember that the Kotlin version of the adapter code is quite short - each function is only a few lines. It's at ths scale that I want you to operate - only a few lines for each.

To be specific, I've asked you to produce two classes, one of which contains three functions. The first class is the `ViewHolder`:

```
CLASS ViewHolder
    GET references to all relevant views
ENDCLASS
```

To write this you need some references to the `View`. I've directed you to write your `View` using HTML, and you likely declared some IDs in your HTML to uniquely identify the HTML elements. For the `Adapter` you'll need to use the syntax of your chosen programming language to create the `ViewHolder` class and declare appropriate variable names (i.e. class members) in that class that match the views declared in HTML (by ID). Something like the following:

```
CLASS ViewHolder
    public string studentName = HTML.student-name
    //... More here...
ENDCLASS
```

In the example the syntax is somewhat Java-like, and might not conform to your language of choice. The `HTML.student-name` element isn't a 'real' thing however, we're just making some assumptions about how you *might* be able to access HTML elements *if* there was such a framework connecting your language and HTML. 

For the rest of the `Adapter` class as you'll take a very similar approach, but this time you'll need to declare some functions. These functions should be written in the programming language of your choice and should be syntactically correct.

For the first line:

```
CLASS Adapter
    GET dataset from model
```

how you write it depends on how you defined your `Model`, but it should be something like creating a new instance of your model class (i.e. `var model = new Model(...)`).

For the last function: 

```
FUNCTION get dataset size
    RETURN size of dataset
ENDFUNCTION
```

you'll use the instantiated model to get the dataset size (i.e. something like `return model.size()`).

The other two functions: 

```
FUNCTION create a ViewHolder instance
    RETURN the ViewHolder instance
ENDFUNCTION

FUNCTION bind data to ViewHolder instance
    GET a ViewHolder instance
    SET data from dataset to appropriate view
ENDFUNCTION
```

 aren't necessarily a lot more complex. Creating the `ViewHolder` instance again involves declaring an instance of your `ViewHolder` class and returning it (like you did with your `Model` class). While binding data involves using that declared `ViewHolder` instance and the declared `Model` instance and connecting them through assignment statements (i.e. `viewHolder.studentName = model.studentName`). Not many lines of code are needed here - in particular, not many more than you have data points.