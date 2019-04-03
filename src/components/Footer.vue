<template>
  <footer>
    <div class="container">
      <div class="row">
        <div class="col-md-4">
          <span class="copyright">{{ FooterText }}</span>
        </div>
        <div class="col-md-4">
          <ul class="list-inline social-buttons">
            <li class="list-inline-item">
              <a v-bind:href="LinkUrlTwitter" target="_blank">
                <i class="fab fa-twitter"></i>
              </a>
            </li>
            <li class="list-inline-item">
              <a v-bind:href="LinkUrlFacebook" target="_blank">
                <i class="fab fa-facebook-f"></i>
              </a>
            </li>
            <li class="list-inline-item">
              <a v-bind:href="LinkUrlLinkedin" target="_blank">
                <i class="fab fa-linkedin-in"></i>
              </a>
            </li>
          </ul>
        </div>
        <div class="col-md-4">
          <ul class="list-inline quicklinks">
            <li class="list-inline-item">
              <a v-bind:href="LinkPrivacy" target="_blank">Privacy Policy</a>
            </li>
            <li class="list-inline-item">
              <a v-bind:href="LinkTerms" target="_blank">Terms of Use</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      FooterText: 'Copyright \u00A9 Your Website 2019',
      LinkUrlTwitter: 'https://twitter.com',
      LinkUrlFacebook: 'https://www.facebook.com',
      LinkUrlLinkedin: 'https://linkedin.com/in/victoria-a-ivanova/',
      LinkPrivacy: '#',
      LinkTerms: '#',
    };
  }
};
</script>

<style scoped>
footer {
	padding: 25px 0;
	text-align: center;
}

footer span.copyright {
	font-size: 90%;
	line-height: 40px;
  text-transform: none;
  color: #fed136;
	font-family: Montserrat, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
}

footer ul.quicklinks {
	font-size: 90%;
	line-height: 40px;
	margin-bottom: 0;
	text-transform: none;
	font-family: Montserrat, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
}

ul.social-buttons {
	margin-bottom: 0;
}

ul.social-buttons li a {
	font-size: 20px;
	line-height: 33px;
	display: block;
	width: 30px;
	height: 30px;
	-webkit-transition: all .3s;
	transition: all .3s;
	color: #fff;
	border-radius: 100%;
	outline: 0;
	background-color: #fed136;
}

ul.social-buttons li a:active,
ul.social-buttons li a:focus,
ul.social-buttons li a:hover {
	background-color: #eab914;
}
</style>
