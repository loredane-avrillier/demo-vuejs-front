<template>
  <div class="container">
    <div>
      <h1 class="title">Accueil</h1>
    </div>
    <div class="home-content">
       <b-card :key="article.id" v-for="article in articles"  :title="article.title" :img-src="url + article.img" img-alt="Image" img-top>
        <b-card-text>{{article.content}}</b-card-text>
        <template v-slot:footer>
          <small class="text-muted">Voir plus</small>
        </template>
      </b-card>
      
       <b-card title="Title" img-src="~/assets/images/guts.jpg" img-alt="Image" img-top>
        <b-card-text>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis cursus justo. Nunc a pulvinar ante, a faucibus diam. Mauris vestibulum tempor leo nec venenatis. Fusce at nisl arcu. Sed nisl felis, auctor sit amet auctor id, accumsan sed nisi. Quisque feugiat pulvinar purus. Nunc id sem tristique, condimentum enim et, sagittis enim. Quisque rhoncus tempor ante lobortis porttitor. Vestibulum sapien ipsum, congue non commodo id, volutpat ac tellus.</b-card-text>
        <template v-slot:footer>
          <small class="text-muted">Voir plus</small>
        </template>
      </b-card>
      
      <!-- 
      <b-card title="Title" img-src="~/assets/images/guts.jpg" img-alt="Image" img-top>
        <b-card-text>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis cursus justo. Nunc a pulvinar ante, a faucibus diam. Mauris vestibulum tempor leo nec venenatis. Fusce at nisl arcu. Sed nisl felis, auctor sit amet auctor id, accumsan sed nisi. Quisque feugiat pulvinar purus. Nunc id sem tristique, condimentum enim et, sagittis enim. Quisque rhoncus tempor ante lobortis porttitor. Vestibulum sapien ipsum, congue non commodo id, volutpat ac tellus.</b-card-text>
        <template v-slot:footer>
          <small class="text-muted">Voir plus</small>
        </template>
      </b-card>
      <b-card title="Title" img-src="~/assets/images/berserk.png" img-alt="Image" img-top>
        <b-card-text>Nunc turpis lectus, commodo porta ante vehicula, aliquet vulputate lacus. Morbi vestibulum hendrerit tristique. Nam feugiat elementum vehicula. Nunc massa felis, rhoncus ut maximus vitae, sagittis eu massa. Fusce tincidunt pulvinar cursus. Integer lacinia lectus at ex pretium rutrum. Aenean ullamcorper eleifend enim nec ullamcorper. Quisque iaculis sem vitae ante imperdiet, vitae lacinia diam lobortis.</b-card-text>
        <template v-slot:footer>
          <small class="text-muted">Voir plus</small>
        </template>
      </b-card>
      <b-card title="Title">
        <b-card-text>Suspendisse feugiat malesuada massa, in venenatis nibh interdum non. Nullam et ex eget ipsum iaculis feugiat. Nullam ullamcorper ac libero quis mattis. Cras volutpat, odio vel ultricies feugiat, ante metus ornare enim, eu luctus ligula sem a nisl. Nunc luctus leo sit amet nunc rutrum, eu vulputate tellus scelerisque. Cras sodales felis non eros condimentum, non finibus mi pulvinar. Praesent ultricies nunc vitae condimentum finibus. Nam ligula felis, tempor nec tristique in, congue quis orci. Pellentesque cursus condimentum dolor, quis volutpat dui dignissim eget.</b-card-text>
        <template v-slot:footer>
          <small class="text-muted">Voir plus</small>
        </template>
      </b-card>
      <b-card>
        <b-card-title>Title</b-card-title>
        <b-card-text>Donec semper ante vitae pellentesque euismod. Fusce ex ipsum, viverra non lacus eget, commodo iaculis ante. Proin a pretium nunc. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras tempus quis massa auctor mattis. Mauris pretium in arcu non tempor. Nam gravida ipsum non ornare imperdiet. Vivamus et congue felis, at tincidunt diam. Nulla erat nisi, ultricies at dictum ac, laoreet a felis. Sed ligula elit, sodales eget dictum at, convallis sit amet elit. Aliquam erat volutpat. Aenean id nisl est.</b-card-text>
        <b-card-text class="small text-muted">Voir plus</b-card-text>
      </b-card>
      <b-card>
        <b-card-title>Title</b-card-title>
        <b-card-text>Donec semper ante vitae pellentesque euismod. Fusce ex ipsum, viverra non lacus eget, commodo iaculis ante. Proin a pretium nunc. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras tempus quis massa auctor mattis. Mauris pretium in arcu non tempor. Nam gravida ipsum non ornare imperdiet. Vivamus et congue felis, at tincidunt diam. Nulla erat nisi, ultricies at dictum ac, laoreet a felis. Sed ligula elit, sodales eget dictum at, convallis sit amet elit. Aliquam erat volutpat. Aenean id nisl est.</b-card-text>
        <b-card-text class="small text-muted">Voir plus</b-card-text>
      </b-card>
      <b-card>
        <b-card-title>Title</b-card-title>
        <b-card-text>Praesent hendrerit consectetur euismod. Phasellus faucibus nulla magna. Vivamus malesuada at arcu a elementum. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Praesent ut mollis ex, sed facilisis ligula. Mauris nibh augue, rhoncus quis posuere vitae, ultricies eu augue. Aliquam placerat dolor quis aliquam mollis. Nunc feugiat elit in accumsan posuere. Nunc efficitur ac felis quis tristique. Vestibulum sit amet quam vitae tortor rhoncus fringilla. In bibendum tortor mauris, sed pulvinar turpis fringilla et. Nulla sollicitudin sodales ligula, at interdum enim mattis a.</b-card-text>
        <b-card-text class="small text-muted">Voir plus</b-card-text>
      </b-card>
      <b-card>
        <b-card-title>Title</b-card-title>
        <b-card-text>Praesent hendrerit consectetur euismod. Phasellus faucibus nulla magna. Vivamus malesuada at arcu a elementum. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Praesent ut mollis ex, sed facilisis ligula. Mauris nibh augue, rhoncus quis posuere vitae, ultricies eu augue. Aliquam placerat dolor quis aliquam mollis. Nunc feugiat elit in accumsan posuere. Nunc efficitur ac felis quis tristique. Vestibulum sit amet quam vitae tortor rhoncus fringilla. In bibendum tortor mauris, sed pulvinar turpis fringilla et. Nulla sollicitudin sodales ligula, at interdum enim mattis a.</b-card-text>
        <b-card-text class="small text-muted">Voir plus</b-card-text>
      </b-card>
      <b-card>
        <b-card-title>Title</b-card-title>
        <b-card-text>Praesent hendrerit consectetur euismod. Phasellus faucibus nulla magna. Vivamus malesuada at arcu a elementum. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Praesent ut mollis ex, sed facilisis ligula. Mauris nibh augue, rhoncus quis posuere vitae, ultricies eu augue. Aliquam placerat dolor quis aliquam mollis. Nunc feugiat elit in accumsan posuere. Nunc efficitur ac felis quis tristique. Vestibulum sit amet quam vitae tortor rhoncus fringilla. In bibendum tortor mauris, sed pulvinar turpis fringilla et. Nulla sollicitudin sodales ligula, at interdum enim mattis a.</b-card-text>
        <b-card-text class="small text-muted">Voir plus</b-card-text>
      </b-card>
      <b-card>
        <b-card-title>Title</b-card-title>
        <b-card-text>Praesent hendrerit consectetur euismod. Phasellus faucibus nulla magna. Vivamus malesuada at arcu a elementum. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Praesent ut mollis ex, sed facilisis ligula. Mauris nibh augue, rhoncus quis posuere vitae, ultricies eu augue. Aliquam placerat dolor quis aliquam mollis. Nunc feugiat elit in accumsan posuere. Nunc efficitur ac felis quis tristique. Vestibulum sit amet quam vitae tortor rhoncus fringilla. In bibendum tortor mauris, sed pulvinar turpis fringilla et. Nulla sollicitudin sodales ligula, at interdum enim mattis a.</b-card-text>
        <b-card-text class="small text-muted">Voir plus</b-card-text>
      </b-card>
      <b-card
        title="Title"
        img-src="~/assets/images/stained-glass-1589648_1920.jpg"
        img-alt="Image"
        img-top
      >
        <b-card-text>
          This is a wider card with supporting text below as a natural lead-in to additional content.
          This content is a little bit longer.
        </b-card-text>
        <template v-slot:footer>
          <small class="text-muted">Voir plus</small>
        </template>
      </b-card>
      <b-card title="Title" img-src="~/assets/images/casacop.jpg" img-alt="Image" img-top>
        <b-card-text>
          This is a wider card with supporting text below as a natural lead-in to additional content.
          This content is a little bit longer.
        </b-card-text>
        <template v-slot:footer>
          <small class="text-muted">Voir plus</small>
        </template>
      </b-card>
      <b-card title="Title">
        <b-card-text>
          This is a wider card with supporting text below as a natural lead-in to additional content.
          This content is a little bit longer.
        </b-card-text>
        <template v-slot:footer>
          <small class="text-muted">Voir plus</small>
        </template>
      </b-card>
     --></div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      articles: [
        {
          id: 1,
          slug: "random",
          title: "Titre article 1",
          content: "Praesent hendrerit consectetur euismod. Phasellus faucibus nulla magna. Vivamus malesuada at arcu a elementum. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Praesent ut mollis ex, sed facilisis ligula. Mauris nibh augue, rhoncus quis posuere vitae, ultricies eu augue. Aliquam placerat dolor quis aliquam mollis. Nunc feugiat elit in accumsan posuere. Nunc efficitur ac felis quis tristique. Vestibulum sit amet quam vitae tortor rhoncus fringilla. In bibendum tortor mauris, sed pulvinar turpis fringilla et. Nulla sollicitudin sodales ligula, at interdum enim mattis a.",
          img: "guts.jpg"
        },
        {
          id:2,
          slug:"article 2",
          title: "Titre article 2",
          content: "Praesent hendrerit consectetur euismod. Phasellus faucibus nulla magna. Vivamus malesuada at arcu a elementum. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Praesent ut mollis ex, sed facilisis ligula. Mauris nibh augue, rhoncus quis posuere vitae, ultricies eu augue. Aliquam placerat dolor quis aliquam mollis. Nunc feugiat elit in accumsan posuere. Nunc efficitur ac felis quis tristique. Vestibulum sit amet quam vitae tortor rhoncus fringilla. In bibendum tortor mauris, sed pulvinar turpis fringilla et. Nulla sollicitudin sodales ligula, at interdum enim mattis a.",
          img: "berserk.png"
        },
        {
          id:3,
          slug: "article 3",
          title: "Titre article 3",
          content: "Praesent hendrerit consectetur euismod. Phasellus faucibus nulla magna. Vivamus malesuada at arcu a elementum. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Praesent ut mollis ex, sed facilisis ligula. Mauris nibh augue, rhoncus quis posuere vitae, ultricies eu augue. Aliquam placerat dolor quis aliquam mollis. Nunc feugiat elit in accumsan posuere. Nunc efficitur ac felis quis tristique. Vestibulum sit amet quam vitae tortor rhoncus fringilla. In bibendum tortor mauris, sed pulvinar turpis fringilla et. Nulla sollicitudin sodales ligula, at interdum enim mattis a.",
          img: "stained-glass-1589648_1920.jpg"
        }

      ]
    };
  },
  computed: {
    url: function() {
      return `/_nuxt/assets/images/`;
    }
  }
};
</script>
<style scoped>
.container {
  margin: 2em auto;
  min-height: 100vh;
}
.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 2em;
  color: #35495e;
  letter-spacing: 1px;
  text-align: left;
}
.home-content {
  display: flex;
  flex-wrap: wrap;
}
.home-content .card {
  width: calc(100% / 3);
  padding: 1em;
}
</style>
