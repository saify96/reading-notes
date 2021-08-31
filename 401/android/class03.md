# Dynamic lists with RecyclerView

- RecyclerView makes it easy to efficiently display large sets of data.You supply the data and define how each item looks, and the RecyclerView library dynamically creates the elements when they're needed.

- RecyclerView recycles those individual elements.

- RecyclerView doesn't destroy its view. Instead, RecyclerView reuses the view for new items that have scrolled onscreen. 


- Several different classes work together to build your dynamic list.

  - RecyclerView is the ViewGroup that contains the views corresponding to your data. 

  - Each individual element in the list is defined by a view holder object.

  - You define the view holder by extending RecyclerView.ViewHolder.


  - The RecyclerView requests those views, and binds the views to their data, by calling methods in the adapter. You define the adapter by extending RecyclerView.Adapter.


  - The layout manager arranges the individual elements in your list. 


- Steps for implementing your RecyclerView

  - decide what the list or grid is going to look like.
  - Design how each element in the list is going to look and behave.
  - Define the Adapter that associates your data with the ViewHolder views.

- The items in your RecyclerView are arranged by a LayoutManager class. The RecyclerView library provides three layout managers

  - LinearLayoutManager arranges the items in a one-dimensional list.

  - GridLayoutManager arranges all items in a two-dimensional grid:

  - StaggeredGridLayoutManager is similar to GridLayoutManager,the result is that the items in a row or column can end up offset from each other.

