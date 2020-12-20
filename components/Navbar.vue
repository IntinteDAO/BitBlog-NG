<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <NuxtLink to="/">
        <a class="navbar-item">
          Intinte BitBlog
        </a>
      </NuxtLink>

      <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbarIntinte">
        <span aria-hidden="true" />
        <span aria-hidden="true" />
        <span aria-hidden="true" />
      </a>
    </div>

    <div id="navbarIntinte" class="navbar-menu">
      <div class="navbar-start" />
      <div class="navbar-end">
        <div class="navbar-item">
          <div class="buttons">
            <NuxtLink to="/signup">
              <a class="button is-primary">
                <strong>Sign up</strong>
              </a>
            </NuxtLink>
            <NuxtLink to="/login">
              <a class="button is-light">
                Log In
              </a>
            </NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  mounted () {
    const $navbarBurgers = Array.prototype.slice.call(document.querySelectorAll('.navbar-burger'), 0)

    if ($navbarBurgers.length === 0) {
      return false
    }

    $navbarBurgers.forEach((el) => {
      el.addEventListener('click', () => {
        const target = el.dataset.target
        const $target = document.getElementById(target)
        el.classList.toggle('is-active')
        $target.classList.toggle('is-active')
      })
    })
  }
}
</script>

<style scoped>
a {
  color: inherit;
  user-select: none;
}
</style>
