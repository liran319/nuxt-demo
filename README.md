# nuxt-demo

> A project to reproduct [BackgroundImage url will be added a '=' at the end of url params when run build #9064](https://github.com/nuxt/nuxt.js/issues/9064)


## Build Setup
```
nuxt: 2.15.3
node: v12.19.0
```

```bash
# install dependencies
$ npm install

# build for production and launch server
$ npm run build

```

Check below file:

```
/.nuxt/dist/client/css/xxxxx.css
```

And find encoded css likes this:
```
.class-a[data-v-11a7bbfe]{
  background-image:url(http://abc.xyz.jpg/?foo%2Fbar=)
}
```


