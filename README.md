# vue-pagination
Vue pagination component for use with Bootstrap and Laravel pagination.
(Looking for maintainer to upgrade it)

* [Vue.js](http://vuejs.org/) (tested with 1.0.16).
* [Bootstrap CSS](http://getbootstrap.com/) (tested with 3.3.6)

#Installation

``` npm install vue-laravel-pagination```

```js

// You have to add this package as component to your vuejs installation
Vue.component('pagination', require('vue-laravel-pagination'));
```

#Usage
For making this component to work you need to provide an pagination object with these data members (all required)

```js
  pagination: {
      total: 0,  // total number of elements or items
      per_page: 12, // items per page
      current_page: 1, // current page (it will be automatically updated when users clicks on some page number).
      total_pages: 10 // total pages in record
  }
  
```
Note that you must set ```current_page``` to 1 initially.

### Example

```html

  <pagination :pagination="pagination" navClass="anyclass" size="pagination-sm" :callback="loadData" :offset="3"></pagination>

  will gerenate like 

  <nav class="anyclass">
  <ul class="pagination pagination-sm">
    <li>
      ...
    </li>
  </ul>
</nav>

```

#### Options
| Name          | Type     | Default | Required | Description
| :------------ | :--------| :-------| :--------| :-----------
| pagination    | Object   |         | true     | Pagination object used to create pagination
| callback      | Function |         | true     | Callback function used to load data for selected page
| offset        | Number   | 4       | false    | Left and right offset of pagination numbers to display
| navClass      | String   |         | false    | Assign a class to your nav element of pagination
| size          | String   |         | false    | Give bootstrap or custom class for sizing your pagination


I will update more info soon...

