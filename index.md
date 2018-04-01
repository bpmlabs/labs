---
layout: index
---
<div class="copy">
  <h2>{{ site.data.app.title }}</h2>
  <p>{{ site.data.app.description | markdownify }}</p>
  <h2>The Best of Both Worlds.</h2>
  <p>{{ site.data.app.combination }}</p>
  <div class="bennies">
    <div class="benefits">
      <h3>Static Sites</h3>
      <hr>
      <ul>
          {% for benefit in site.data.app.staticBenefits %}
            <li>{{ benefit | capitalize }}</li>
          {% endfor %}
      </ul>
    </div>
    <div class="benefits">
      <h3>Client-Side JS</h3>
      <hr>
      <ul>
          {% for benefit in site.data.app.dynamicBenefits %}
            <li>{{ benefit | capitalize }}</li>
          {% endfor %}
      </ul>
    </div>
  </div>
  <p class="environment">*Enable Javascript to see the page rendered with Vue.</p>
  <h3>Direct text</h3>
  <p>[This Repo](https://github.com/pegalabs/labs) is a bare-bones template for building static sites that leverage a client-side JS framework for dynamic functionality. It uses [NPM](https://www.npmjs.com/), [Webpack](https://webpack.js.org), [Vue](https://vuejs.org), and [Jekyll](https://jekyllrb.com). It uses **NPM (and Bundler)** to manage the project's dependencies, and improve the development workflow. It uses **Webpack** to roll up and transpile all the individual modules and components into a single bundeled JS file. It uses **Jekyll** to bring it all together, build the site, and serve an initial static file to the browser. It uses **Vue** to render pages on the client side (if JS is supported), and provide any additional dynamic functionality that may be needed.</p>
</div>