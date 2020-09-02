<template>
  <div>
    <footer>
      <ul
        class="bg-light m-0 p-3 h-100 d-flex list-unstyled justify-content-between align-items-center"
      >
        <li class="h-100"> IMAGE
        </li>
        <li class="h-100">
          <n-link to="#">Nous contacter</n-link>
        </li>
        <li class="h-100">
          <n-link to="#">Aide</n-link>
         
        </li>
        <li class="h-100">
          <a href="#"> LIEN
          </a>
        </li>
        <li class="h-100 link-e-plans">
          <a href="#">
          LIEN
          </a>
        </li>
      </ul>
    </footer>
  </div>
</template>

<script>
export default {
  name: "AppFooter"
};
</script>

<style>
footer img {
  width: 60px;
}
footer .link-e-plans img {
  width: 100px;
}
footer a, footer
a:hover {
  text-transform: uppercase;
  font-weight: 500;
}
</style>