<template>
<p>SAimple text</p>
</template>
<script>
export default {
  dta() {
    return {
      activePage: 0,
      page: [
        {
          link: {text: 'Home', url: 'index.html'},
          pageTitle: 'Home Page',
          content: 'This is the home content'
        },
        {
          link: {text: 'About', url: 'about.html'},
          pageTitle: 'About Page',
          content: 'This is the about content'
        },
        {
          link: {text: 'Contact', url: 'content.html'},
          pageTitle: 'Contact Page',
          content: 'This is the content content'
        }
      ]
    }
  }
}
</script>