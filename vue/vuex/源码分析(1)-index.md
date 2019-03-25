#### 源码

``` javascript
import { Store, install } from './store'
import { mapState, mapMutations, mapGetters, mapActions, createNamespacedHelpers } from './helpers'

export default {
  Store,
  install,
  version: '__VERSION__',
  mapState,
  mapMutations,
  mapGetters,
  mapActions,
  createNamespacedHelpers
}
```

#### 分析

这是`vuex`对外提供的接口, 其中`version`是`vuex`的版本，`mapState`, `mapMutations`, `mapGetters`, `mapActions`, `createNamespacedHelpers`,是工具函数，我们暂时先不关注。

我们可以看到`Store`, `install`都是从`./store`导出的，因此需要先分析`./store`.