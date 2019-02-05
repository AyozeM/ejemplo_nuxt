<template>
  <b-navbar toggleable="md" type="dark" variant="info">
    <b-navbar-toggle target="nav_collapse"/>

    <b-navbar-brand to="/">Web</b-navbar-brand>

    <b-collapse id="nav_collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item to="informacion">Informacion</b-nav-item>
        <b-nav-item to="quienes-somos">Quienes somos</b-nav-item>
        <b-nav-item to="contacto">Contacto</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>
