<script lang="ts">
  export let navlists = [];
  export let header;
</script>

<section id="nav-bar">
  <nav class="navbar main-bg-color navbar-expand-md navbar-dark">
    <a class="navbar-brand company_brand" href="/">
      {header}
    </a>
    <!-- <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarNav"
      aria-controls="navbarNav"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon" />
    </button> -->
    <div class="topnav" id="navbarNav">
      <ul class="navbar-nav ml-auto">
        {#each navlists as list}
          <li class="nav-item">
            <a class="nav-link" href={list.url}>{list.label}</a>
          </li>
        {/each}
      </ul>
    </div>
  </nav>
</section>

<style>
    #nav-bar {
      position: sticky;
      top: 0;
      z-index: 10;
    }
  
    .navbar {
      padding: 0 20px !important;
    }
  
    .navbar-nav li {
      padding: 0 0 0 20px;
    }
  
    .navbar-nav li a {
      font-weight: 600;
      text-transform: uppercase;
      float: right;
      text-align: left;
      /* color: #000 */
    }

    .nav-link {
        color: #000
    }

    .nav-link:hover {
      color: #080
    }
  </style>