<template>
  <div class="section">
    <div class="container">
      <div class="columns">
        <div
          v-for="post in posts"
          :key="post.id"
          class="column"
        >
          <strong> {{ post.title }} </strong>
          {{ post.desc }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  transition: 'page',
  data () {
    return {
      posts: [
        {
          id: 0,
          title: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
          desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit' +
          'sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.' +
          'Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris' +
          'nisi ut aliquip ex ea commodo consequat.'
        },
        {
          id: 1,
          title: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
          desc: 'Diam vulputate ut pharetra sit amet aliquam. Aliquam ut porttitor' +
          'leo a diam sollicitudin tempor id. Sit amet risus nullam eget' +
          'felis eget nunc lobortis mattis. Vitae turpis massa sed elementum tempus' +
          'egestas sed. Duis tristique sollicitudin nibh sit amet commodo nulla.' +
          'Ornare arcu odio ut sem nulla pharetra diam sit.'
        },
        {
          id: 2,
          title: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
          desc: 'Vitae congue mauris rhoncus aenean vel elit. Etiam sit amet' +
          'nisl purus in mollis nunc sed. Tellus in metus vulputate eu scelerisque' +
          'felis imperdiet. Quis commodo odio aenean sed.'
        }
      ]
    }
  }
}
</script>
