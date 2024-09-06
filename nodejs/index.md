### 仓库源

```shell
npm ---------- https://registry.npmjs.org/
yarn --------- https://registry.yarnpkg.com/
tencent ------ https://mirrors.cloud.tencent.com/npm/
cnpm --------- https://r.cnpmjs.org/
taobao ------- https://registry.npmmirror.com/
npmMirror ---- https://skimdb.npmjs.com/registry/

```



### npm安装依赖报错

npm安装依赖的时候报错超时，如下：

```shell
npm error code ECONNRESET
npm error syscall read
npm error errno ECONNRESET
npm error network Invalid response body while trying to fetch https://registry.npmjs.org/element-plus: read ECONNRESET
npm error network This is a problem related to network connectivity.
npm error network In most cases you are behind a proxy or have bad network settings.
npm error network
npm error network If you are behind a proxy, please make sure that the
npm error network 'proxy' config is set properly.  See: 'npm help config'
```

解决

```shell
npm config set registry https://registry.npmmirror.com
```

