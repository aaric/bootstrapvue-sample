# bootstrapvue-sample

## Project setup

```bash
npm install
```

### Compiles and hot-reloads for development

```bash
npm run serve
```

### Compiles and minifies for production

```bash
npm run build
```

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).


## BootstrapVue setup

```bash
npm install --save-exact bootstrap-vue bootstrap axios
```

## Docker preparation

```bash
# set npm config
npm config set cache /home/jenkins/node_cache
npm config set prefix /home/jenkins/node_global
npm config set registry https://registry.npm.taobao.org

# get project version
node -p "require('./package.json').version"

# harbor robot login
echo '<token>' | docker login s1:5000 -u 'robot$<name>' --password-stdin
```

