# vue-app-example

PoC app to test [Vue.js](https://vuejs.org/) framework

### Getting Started

0. Install project dependencies:
```bash
npm install && bower install
```

1. Add this line to your `hosts` file:
```
127.0.0.1	vue-app-example.dev
```

2. Build project for both client & server environments:
```bash
npm run build:dev
```

3. Build & run docker image using Docker Compose:
```bash
docker-compose up --build
```

Now you can open [http://vue-app-example.dev](http://vue-app-example.dev)
application in browser.

To test Server-Side Rendering, you can emulate search bot request:
```bash
curl --header "User-Agent: Googlebot" http://vue-app-example.dev/
```
or directly do request to Express server:
```bash
curl http://vue-app-example.dev:8080/
```

### Useful Resources for Beginners

- Vue components style guide
  - https://github.com/pablohpsilva/vuejs-component-style-guide
  - http://vuetips.com/vue-component-style-guide
- Vue plugins catalog: https://github.com/vuejs/awesome-vue
- Chai BDD: http://chaijs.com/api/bdd/
- Form validation plugin: http://vee-validate.logaretm.com/
- Mocking vue-resource requests while unit-testing: http://matthiashager.com/blog/mocking-http-requests-with-vuejs
- Vue dev tools Chrome extension: https://github.com/vuejs/vue-devtools
- https://github.com/vuejs/vue-hackernews-2.0

### Future Roadmap

- Stylus
- http://haml.info/
- https://ssr.vuejs.org/en/
- [vue-kindergarten](https://github.com/JiriChara/vue-kindergarten)
- Nuxt.js
- [Weex](https://github.com/weexteam/weex-vue-framework)
- [av-ts](https://github.com/HerringtonDarkholme/av-ts): https://herringtondarkholme.github.io/2016/10/03/vue2-ts2/
- https://github.com/rowanwins/vue-dropzone

### Known Issues

- Rolling back HMR updates (**temporarily postponed**)
