# Taro1.x snippets

丰富vscode的代码对于Taro框架的代码提示功能，$1表示创建代码片段后光标第一个所在区域，按tab键会依次切换到下一个位置

## 代码片段

### taro-page

```javascript
import Taro, { Component, Config } from '@tarojs/taro'
import { View } from '@tarojs/components'
import getShareCommon from '@/utils/share'

type IState = {}

/**
 * @cmdName {$2} $3 
 */
export default class  extends Component<{}, IState> {
  config: Config = {
    navigationBarTitleText: '$4',
    navigationBarTextStyle: 'black'
  }

  state: IState = {
    
  }

  componentWillMount() {}

  componentDidShow() {}

  onShareAppMessage() {
    return getShareCommon('$4', '$2')
  }

  render() {
    return (
      <View>$5</View>
    )
  }
}
```

### taro-component

```javascript
import Taro, { Component } from '@tarojs/taro'
import { View } from '@tarojs/components'

type IState = {}

type IProps = {}

export default class $1 extends Component<IProps, IState> {
  state: IState = {}

  componentWillMount() {
    
  }

  componentDidShow() {
    
  }

  componentWillReceiveProps(nextProps) {
    
  }

  render() {
    return (
      <View>$2</View>
    )
  }
}
```

### eventCenter.on

```javascript
Taro.eventCenter.on('$1', $2)
```

### eventCenter.off

```javascript
Taro.eventCenter.off('$1', $2)
```

### showToast

```javascript
Taro.showToast({ icon: '$1', title: '$2' })
```

### showLoading

```javascript
Taro.showLoading({ title: '$2' })
```

### showModal

```javascript
Taro.showModal({
  title: '$1',
  content: '$2'
})
```

### uploadFile

```javascript
Taro.uploadFile({
  url: '$1',
  name: '$2',
  filePath: '$3'
})
```

### downloadFile

```javascript
Taro.downloadFile({
  url: '$1',
  success(resp) {
    $2
  }
})
```

### Taro.setStorage

```javascript
Taro.setStorage({
  key: '$1',
  data: $2
})
```


### getLocation

```javascript
Taro.getLocation({
  type: 'gcj02',
  success(resp) {
    $1
  }
})
```

### openLocation

```javascript
Taro.openLocation({
  latitude: $1,
  longitude: $2
})
```

### onShareAppMessage

```javascript
onShareAppMessage () {
  return {
    title: '$1',
  }
}
```

### componentWillMount

```javascript
componentWillMount() {
  $1
}
```

......