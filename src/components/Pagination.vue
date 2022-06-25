<template>
  <footer>
    <div class="card-footer">
      <div class="card-text-footer">
        <h2 class="card-title">This is Exam Question 3 "Pagination"</h2>
        <div class="card-text" style="margin-bottom: 15px">
          If you want to see the results of Problem 4, change the Pagination to
          the next page.
          <div class="pagination-center">
            <div class="pagination">
              <!-- <router-link to="/">&laquo;</router-link> |
            <router-link to="/FormButton">1</router-link>
            <router-link to="/FormLayout">2</router-link>
            <router-link to="/contract">&raquo;</router-link>             -->
              <a>&laquo;</a>
              <a onclick="openCity(event, 'FormButton')">1</a>
              <a onclick="openCity(event, 'Pagination')">2</a>
              <a>&raquo;</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>


