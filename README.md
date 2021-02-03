# Taro1.x snippets

vscode的代码提示功能，$1表示光标第一个所在区域，按tab键会依次切换到下一个位置

## 代码片段

### taroc

```javascript
import Taro, { Component } from '@tarojs/taro'
import { View } from '@tarojs/components'

export default class $1 extends Component {
  render () {
    return (
      <View>$2</View>
    )
  }
}
```

### taro-config

```javascript
config = {
  navigationBarTitleText: '$1',
  navigationBarTextStyle: 'black'
}
```

### setState

```javascript
this.setState({ $1: $2 })
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
  success(resp: { latitude: number, longitude: number, speed: number, accuracy: number, altitude: number, verticalAccuracy: number, horizontalAccuracy: number }) {
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