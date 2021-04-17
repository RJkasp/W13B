<template>
  <div id="app">
    <button @click='changeLayout'>Toggle</button>
    <section id="tweets">
      <!-- Loop thru objects inside tweetsdata-->
      <article v-for="tweet in tweetsData" :key="tweet">
        <h3>{{tweet.user}}</h3>
        <p>{{tweet.content}}</p>
        <p>{{tweet.date}}</p>
      </article>
    </section>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return{
      //array of tweets content,title and date
    tweetsData: [
      {
        content:`I’m not saying over a year in quarantine has messed with me but a tiny lizard got into my apartment and I was like, “oh good, you made it.”`,
        user: 'RJ Kasprick',
        date: '04/16/2021',
      },
        {
        content:`I’m not saying over a year in quarantine has messed with me but a tiny lizard got into my apartment and I was like, “oh good, you made it.”`,
        user: 'RJ Kasprick',
        date: '04/16/2021',
      },
        {
        content:`I’m not saying over a year in quarantine has messed with me but a tiny lizard got into my apartment and I was like, “oh good, you made it.”`,
        user: 'RJ Kasprick',
        date: '04/16/2021',
      },
        {
        content:`I’m not saying over a year in quarantine has messed with me but a tiny lizard got into my apartment and I was like, “oh good, you made it.”`,
        user: 'RJ Kasprick',
        date: '04/16/2021',
      },
        {
        content:`I’m not saying over a year in quarantine has messed with me but a tiny lizard got into my apartment and I was like, “oh good, you made it.”`,
        user: 'RJ Kasprick',
        date: '04/16/2021',
      },
        {
        content:`I’m not saying over a year in quarantine has messed with me but a tiny lizard got into my apartment and I was like, “oh good, you made it.”`,
        user: 'RJ Kasprick',
        date: '04/16/2021',
      },
        {
        content:`I’m not saying over a year in quarantine has messed with me but a tiny lizard got into my apartment and I was like, “oh good, you made it.”`,
        user: 'RJ Kasprick',
        date: '04/16/2021',
      },
        {
        content:`I’m not saying over a year in quarantine has messed with me but a tiny lizard got into my apartment and I was like, “oh good, you made it.”`,
        user: 'RJ Kasprick',
        date: '04/16/2021',
      },
        {
        content:`I’m not saying over a year in quarantine has messed with me but a tiny lizard got into my apartment and I was like, “oh good, you made it.”`,
        user: 'RJ Kasprick',
        date: '04/16/2021',
      },
        {
        content:`I’m not saying over a year in quarantine has messed with me but a tiny lizard got into my apartment and I was like, “oh good, you made it.”`,
        user: 'RJ Kasprick',
        date: '04/16/2021',
      }
    ]
   }
   },
   //function for tweets and toggle thru layouts
     methods: {
        changeLayout: function(){
          document.getElementById('tweets').classList.toggle('className');
        },
 }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.className{
    display: grid;
    grid-template-columns: repeat(10, 1fr);
}
</style>
