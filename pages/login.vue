<template>
  <div class="section">
    <div class="container">
      <div class="columns">
        <div class="column">
          <div class="field">
            <label class="label">Login</label>
            <div class="control">
              <input class="input" type="text" placeholder="Text input">
            </div>
          </div>
          <div class="field">
            <p class="control">
              <input class="input" type="password" placeholder="Password">
            </p>
          </div>

          <div class="field is-grouped">
            <div class="control">
              <button class="button is-link">
                Login
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  transition: 'page'
}
</script>
