# vue-pagination
Vue pagination component for use with Bootstrap and Laravel pagination.

* [Vue.js](http://vuejs.org/) (tested with 1.0.16).
* [Bootstrap CSS](http://getbootstrap.com/) (tested with 3.3.6)

All it requires to work is this object and a callback function


### Example
```js
  pagination: {
      total: 0, 
      per_page: 12,
      current_page: 1,
      total_pages: 10
  }
```

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

