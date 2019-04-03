<template>
  <section id="about">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">{{ pageTitle}}</h2>
          <h3 class="section-subheading text-muted">{{ pageQuote }}</h3>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-12">
          <ul class="about">
            <li>
              <div class="about-panel">
                <div class="about-heading">
                  <h4 class="subheading">{{ infoFirstQuote }}</h4>
                </div>
                <div class="about-body">
                  <p class="text-muted">{{ infoFirst }}</p>
                </div>
              </div>
            </li>
            <li class="about-inverted">
              <div class="about-panel">
                <div class="about-heading">
                  <h4 class="subheading">{{ infoSecondQuote }}</h4>
                </div>
                <div class="about-body">
                  <p class="text-muted">{{ infoSecond }}</p>
                </div>
              </div>
            </li>
            <li class="about-inverted">
              <div class="about-image">
                <h4>POWERED
                  <br>BY
                  <br>COFFEE</h4>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
    data() {
			return {
				pageTitle: 'About',
        pageQuote: 'Lorem ipsum dolor sit amet consectetur..',
        infoFirstQuote: 'A rare experience in taste.',
        infoFirst: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sunt ut voluptatum eius sapiente, totam reiciendis temporibus qui quibusdam, recusandae sit vero unde, sed, incidunt et ea quo dolore laudantium consectetur!',
        infoSecondQuote: 'Make more of the moment.',
				infoSecond: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sunt ut voluptatum eius sapiente, totam reiciendis temporibus qui quibusdam, recusandae sit vero unde, sed, incidunt et ea quo dolore laudantium consectetur!',
			}
		}
}
</script>

<style scoped>

.about {
	position: relative;
	padding: 0;
	list-style: none;
}

.about:before {
	position: absolute;
	top: 0;
	bottom: 0;
	left: 40px;
	width: 2px;
	margin-left: -1.5px;
	content: '';
	background-color: #e9ecef;
}

.about>li {
	position: relative;
	min-height: 50px;
}

.about>li:after,
.about>li:about {
	display: table;
	content: ' ';
}

.about>li:after {
	clear: both;
}

.about>li .about-panel {
	position: relative;
	float: right;
	width: 100%;
	padding: 0 20px 0 100px;
	text-align: left;
}

.about>li .about-panel:before {
	right: auto;
	left: -15px;
	border-right-width: 15px;
	border-left-width: 0;
}

.about>li .about-panel:after {
	right: auto;
	left: -14px;
	border-right-width: 14px;
	border-left-width: 0;
}

.about>li .about-image {
	position: absolute;
	z-index: 100;
	left: 0;
	width: 80px;
	height: 80px;
	margin-left: 0;
	text-align: center;
	color: #fff;
	border: 7px solid #e9ecef;
	border-radius: 100%;
	background-color: #fed136;
}

.about>li .about-image h4 {
	font-size: 10px;
	line-height: 14px;
	margin-top: 12px;
}

.about>li.about-inverted>.about-panel {
	float: right;
	padding: 0 20px 0 100px;
	text-align: left;
}

.about>li.about-inverted>.about-panel:before {
	right: auto;
	left: -15px;
	border-right-width: 15px;
	border-left-width: 0;
}

.about>li.about-inverted>.about-panel:after {
	right: auto;
	left: -14px;
	border-right-width: 14px;
	border-left-width: 0;
}

.about>li:last-child {
	margin-bottom: 0;
}

.about .about-heading h4 {
	margin-top: 0;
	color: inherit;
}

.about .about-heading h4.subheading {
	text-transform: none;
}

.about .about-body>p,
.about .about-body>ul {
	margin-bottom: 0;
}

@media (min-width:768px) {
	.about:before {
		left: 50%;
	}
	.about>li {
		min-height: 100px;
	}
	.about>li .about-panel {
		float: left;
		width: 41%;
		padding: 0 20px 20px 30px;
		text-align: right;
	}
	.about>li .about-image {
		left: 50%;
		width: 100px;
		height: 100px;
		margin-left: -50px;
	}
	.about>li .about-image h4 {
		font-size: 13px;
		line-height: 18px;
		margin-top: 16px;
	}
	.about>li.about-inverted>.about-panel {
		float: right;
		padding: 0 30px 20px 20px;
		text-align: left;
	}
}

@media (min-width:992px) {
	.about>li {
		min-height: 150px;
	}
	.about>li .about-panel {
		padding: 0 20px 20px;
	}
	.about>li .about-image {
		width: 150px;
		height: 150px;
		margin-left: -75px;
	}
	.about>li .about-image h4 {
		font-size: 15px;
		line-height: 16px;
		margin-top: 30px;
	}
	.about>li.about-inverted>.about-panel {
		padding: 0 20px 20px;
	}
}

@media (min-width:1200px) {
	
	.about>li .about-panel {
		padding: 0 20px 20px 100px;
	}
	.about>li .about-image {
		width: 130px;
		height: 130px;
    margin-left: -65px;
    margin-top: 60px;
	}
	.about>li .about-image h4 {
		margin-top: 36px;
	}
	.about>li.about-inverted>.about-panel {
		padding: 0 100px 20px 20px;
	}
}

</style>


