<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue'
import { Button } from 'flowbite-vue'
</script>
<template>
  <div class="nav">
    <Navbar>
      <template #logo>
        <NavbarLogo link="https://www.google.com/" alt="Flowbite logo" image-url="https://flowbite.com/docs/images/logo.svg">
          Elva Hijab
        </NavbarLogo>
      </template>
      <template #default="{isShowMenu}">
        <NavbarCollapse :isShowMenu="isShowMenu">
          <NavbarLink is-active>Home</NavbarLink>
          <NavbarLink>Services</NavbarLink>
          <NavbarLink>Pricing</NavbarLink>
          <NavbarLink>Contact</NavbarLink>
        </NavbarCollapse>
      </template>
      <template #right-side>
        <Button gradient="purple-pink">Purple to pink</Button>
      </template>
    </Navbar></div>
</template>

<style>

</style>
