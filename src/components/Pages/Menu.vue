<template>
    <section id="menu">
      <div class="container">
        <div class="row">
          <div class="col-lg-12 text-center" v-for="(obj, key) in pageJSON" :key="key">
            <h2 class="section-heading text-uppercase">{{ obj.pageTitle }}</h2>
            <h3 class="section-subheading text-muted">{{ obj.pageInfo }}</h3>
          </div>
        </div>
        <div class="row text-center">
        <div class="col-md-4" v-for="(obj, key) in menuJSON" :key="key">
            <span class="fa-stack">
              <i class="fas fa-circle fa-stack-2x circle-colour"></i>
              <i class="fas fa-mug-hot fa-stack-1x fa-inverse"></i>
            </span>
            <h4 class="menu-heading">{{ obj.header }}</h4>
            <p class="text-muted">{{ obj.caption }}</p>
        </div>
        </div>
      </div>
    </section> 
</template>

<script>
export default {
    data: () => ({
        menuJSON: [
            {
                header: 'Doppio',
                caption: 'Two shots of espresso. Straight.',
            },
            {
                header: 'Caffe Americano',
                caption: 'Shots of espresso and filtered hot water.',
            },
            {
                header: 'Latte Macchiato',
                caption: 'Foamed whole milk marked with shots of espreso.',
            },
            {
                header: 'Flat White',
                caption: 'Sweet ristretto espresso shots finished with steamed while milk.',
            },
            {
                header: 'Cappuccino',
                caption: 'A shot of espresso topped with a deep layer of foamed milk.',
            },
            {
                header: 'Caffe Latte',
                caption: 'A shot of espresso in steamed milk lightly topped with foam.',
            },
        ],
        pageJSON: [
            {
                pageTitle: 'Menu',
                pageInfo: 'Home of the world’s finest coffees. Let us help you espress yourself.',
            }
        ]
    })
    
}
</script>

<style scoped>

.menu-heading {
	margin: 15px 0;
	text-transform: none;
}

.circle-colour {
    color: #fec503;
}

</style>



