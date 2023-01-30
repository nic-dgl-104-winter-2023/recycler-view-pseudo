# Adapter
The Adapter, in this context, is an Android-specific construct used as part of a [RecyclerView](https://developer.android.com/develop/ui/views/layout/recyclerview) and used by the [RecyclerView class](https://developer.android.com/reference/androidx/recyclerview/widget/RecyclerView) to manage data to be displayed.

The Adapter is where most of the work in *binding* data to views takes place. Typically the goal is [data binding](https://en.wikipedia.org/wiki/Data_binding), which ensures that the data and views are synchronized (but are not the same objects). How data binding is managed is highly platform-dependent.

A ViewHolder class is also included here as a wrapper class for the views.

## Pseudocode
```
CLASS ViewHolder
    GET references to all relevant views
ENDCLASS


CLASS Adapter
    GET dataset from model

    FUNCTION create a ViewHolder instance
        RETURN the ViewHolder instance
    ENDFUNCTION

    FUNCTION bind data to ViewHolder instance
        GET a ViewHolder instance
        SET data from dataset to appropriate view
    ENDFUNCTION

    FUNCTION get dataset size
        RETURN size of dataset
    ENDFUNCTION
ENDCLASS
```