<template>
     <nav class="navbar">
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li>
        <div class="dropdown">
          <a href="#" class="dropbtn">Services</a>
          <div class="dropdown-content">
            <a href="#">Service 1</a>
            <a href="#">Service 2</a>
            <a href="#">Service 3</a>
          </div>
        </div>
      </li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>
</template>

<script>


export default {
  name: 'Navbares',
  components: {
    
  }
}
</script>

<style>
   .navbar {
    text-align: center;
    background-color: #333;
    color: #fff;
    padding: 10px;
    border-radius: 5px;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline;
    margin-right: 60px;
  }

  a {
    text-decoration: none;
    color: #fff;
  }

  /* Dropdown styles */
  .dropdown {
    position: relative;
    display: inline-block;
  }

  .dropbtn {
    cursor: pointer;
  }

  .dropdown-content {
    display: none;
    position: absolute;
    background-color: #333;
    min-width: 100px;
    z-index: 1;
  }

  .dropdown-content a {
    color: #fff;
    padding: 12px 10px;
    text-decoration: none;
    display: block;
  }

  .dropdown-content a:hover {
    background-color: #444;
  }

  .dropdown:hover .dropdown-content {
    display: block;
  }

  .dropdown:hover .dropbtn {
    background-color: #444;
  }
</style>