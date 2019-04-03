<template>
    <section class="bg-light" id="team">
      <div class="container">
        <div class="row">
          <div class="col-lg-12 text-center" v-for="(obj, key) in pageJSON" :key="key">
            <h2 class="section-heading text-uppercase">{{ obj.PageTitle }}</h2>
            <h3 class="section-subheading text-muted">{{ obj.PageInfo}}</h3>
          </div>
        </div>
        <div class="row">
          <div class="col-sm-4" v-for="(obj, key) in teamJSON" :key="key">
            <div class="team-member">
              <h4>{{ obj.Name }}</h4>
              <p class="text-muted">{{ obj.Position }}</p>
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col-lg-8 mx-auto text-center" v-for="(obj, key) in pageJSON" :key="key">
            <p class="large text-muted">{{ obj.TeamResume }}</p>
          </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
    data: () => ({
        teamJSON: [
            {
                Name: 'Rose Hathaway',
                Position: 'Owner',
            },
            {
                Name: 'Lydia Martin',
                Position: 'Pastry Chef',
            },
            {
                Name: 'Scott McCall',
                Position: 'Pastry Chef',
            },
            {
                Name: 'Erica Reyes',
                Position: 'Barista',
            },
            {
                Name: 'Jackson Whittemore',
                Position: 'Barista',
            },
            {
                Name: 'Allison Argent',
                Position: 'Barista',
            },
        ],
        pageJSON: [
            {
                PageTitle: 'Our Amazing Team',
                PageInfo: 'Lorem ipsum dolor sit amet consectetur.',
                TeamResume: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aut eaque, laboriosam veritatis, quos non quis ad perspiciatis, totam corporis ea, alias ut unde.',
            }
        ]
    })
}
</script>

<style scoped>

.team-member {
    margin-bottom:50px;
    text-align:center;
}

.team-member h4 {
    margin-top:25px;
    margin-bottom:0;
    text-transform:none;
    color: #fed136;
}

.team-member p {
    margin-top:0;
}

</style>


