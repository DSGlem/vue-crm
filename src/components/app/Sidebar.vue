<template>
  <ul class="sidenav app-sidenav open">
    <router-link
      v-for="link in links"
      :key="link.url"
      tag="li"
      active-class="class"
      :to="link.url"
    >
      <a href="#" class="waves-effect waves-orange pointer">{{link.title}}</a>
    </router-link>


  </ul>
</template>

<script>
export default {
  data: () => ({
    links: [
      {title: 'Счет', url: '/home'},
      {title: 'История', url: '/history'},
      {title: 'Планирование', url: '/planning'},
      {title: 'Новая запись', url: '/record'},
      {title: 'Категории', url: '/categories'}
    ]
  })
}
</script>