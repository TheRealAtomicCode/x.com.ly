<template>
  <ul id="menu">
    <li><RouterLink to="/">Home</RouterLink></li>
    <li><RouterLink to="/work">Work</RouterLink></li>
    <li><RouterLink to="/contact">Contact</RouterLink></li>
  </ul>
</template>

<style>
#menu {
  margin: 0;
  padding: 0;
  background-color: #191919;
  display: flex;
  justify-content: center;
  align-items: center;
}

#menu li {
  list-style: none;
  display: inline-block;
}

#menu li a {
  text-decoration: none;
  position: relative;
  color: white;
  font-weight: 700;
  font-family: sans-serif;
  display: block;
  overflow: hidden;
  transition: 0.7s all;
  padding: 14px 0px;
  margin: 0px 30px;
  text-transform: uppercase;
}

#menu li a:before {
  content: '';
  width: 3rem;
  position: absolute;
  border-bottom: 8px solid white;
  bottom: 0;
  right: 350px;
  transition: 0.7s all;
}

#menu li a:hover:before {
  right: 0;
}

/* Small Devices */
@media (max-width: 767px) {
  #menu li a {
    font-size: 20px;
  }
}

/* Medium Devices */
@media (min-width: 768px) and (max-width: 1199px) {
  #menu li a {
    font-size: 24px;
  }
}

/* Large Devices */
@media (min-width: 1200px) {
  #menu li a {
    font-size: 30px;
  }
}
</style>