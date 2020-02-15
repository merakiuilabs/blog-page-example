<template>
  <div id="app">
    <navbar></navbar>
    <div class="flex justify-center">
      <div class="flex px-6 py-8 container">
        <div class="w-full lg:w-8/12">
          <div class="flex items-center justify-between">
            <h1 class="text-xl font-bold text-gray-700 md:2xl">Post</h1>
            <post-filter></post-filter>
          </div>
          <div class="mt-6" v-for="post in posts" :key="post.id">
            <post :data="post"></post>
          </div>
          <div class="mt-8">
            <Pagination></Pagination>
          </div>
        </div>
        <div class="pl-8 w-4/12 hidden lg:block">
          <div>
            <h1 class="text-xl font-bold text-gray-700 md:2xl">Authors</h1>
            <users-list></users-list>
          </div>
          <div class="mt-10">
            <h1 class="text-xl font-bold text-gray-700 md:2xl">Categories</h1>
            <categories></categories>
          </div>
          <div class="mt-10">
            <h1 class="text-xl font-bold text-gray-700 md:2xl">Recent Post</h1>
            <recent-post></recent-post>
          </div>
        </div>
      </div>
    </div>
    <simple-footer></simple-footer>
  </div>
</template>

<script>
import Navbar from "./components/navigation-navbar-simple";
import PostFilter from "./components/elements-select-option";
import Post from "./components/elements-blog-post-article-review";
import Pagination from "./components/elements-pagination";
import UsersList from "./components/sections-blog-users-list";
import Categories from "./components/sections-categories-list";
import RecentPost from "./components/sections-recent-article";
import SimpleFooter from "./components/navigation-footer-simple-with-icon";
export default {
  name: 'app',
  components: { Navbar , PostFilter , Post , Pagination , UsersList , Categories , RecentPost , SimpleFooter },
   data() {
    return {
      posts: [
        {
          id: 1,
          date: "Jun 1, 2020",
          tag: "Laravel",
          title: "Build Your New Idea with Laravel Freamwork.",
          body: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora expedita dicta totam aspernatur doloremque. Excepturi iste iusto eos enim reprehenderit nisi, accusamus delectus nihil quis facere in modi ratione libero!",
          image: "https://images.unsplash.com/photo-1492562080023-ab3db95bfbce?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=731&q=80",
          userName:"Alex John"
        },
        {
          id: 2,
          date: "mar 4, 2019",
          tag: "Design",
          title: "Accessibility tools for designers and developers",
          body: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora expedita dicta totam aspernatur doloremque. Excepturi iste iusto eos enim reprehenderit nisi, accusamus delectus nihil quis facere in modi ratione libero!",
          image: "https://images.unsplash.com/photo-1464863979621-258859e62245?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=333&q=80",
          userName:"Jane Doe"
        },
        {
          id: 3,
          date: "Feb 14, 2019",
          tag: "PHP",
          title: "PHP: Array to Map",
          body: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora expedita dicta totam aspernatur doloremque. Excepturi iste iusto eos enim reprehenderit nisi, accusamus delectus nihil quis facere in modi ratione libero!",
          image: "https://images.unsplash.com/photo-1531251445707-1f000e1e87d0?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=281&q=80",
          userName:"Lisa Way"
        },
        {
          id: 4,
          date: "Dec 23, 2018",
          tag: "Django",
          title: "Django Dashboard - Learn by Coding",
          body: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora expedita dicta totam aspernatur doloremque. Excepturi iste iusto eos enim reprehenderit nisi, accusamus delectus nihil quis facere in modi ratione libero!",
          image: "https://images.unsplash.com/photo-1500757810556-5d600d9b737d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=735&q=80",
          userName:"Steve Matt"
        },
        {
          id: 5,
          date: "Mar 10, 2018",
          tag: "Testing",
          title: "TDD Frist",
          body: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora expedita dicta totam aspernatur doloremque. Excepturi iste iusto eos enim reprehenderit nisi, accusamus delectus nihil quis facere in modi ratione libero!",
          image: "https://images.unsplash.com/photo-1502980426475-b83966705988?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=373&q=80",
          userName:"Khatab Wedaa"
        },
      ]
    }
  }
}
</script>

<style>
  @import "assets/css/app.css";
</style>
