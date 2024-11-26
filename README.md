# React Native Stylewind

---

## 📦 安装

通过 npm 或 yarn 安装：

```bash
npm install react-native-stylewind
```

或

```bash
yarn add react-native-stylewind
```

---

### **基本使用**

为组件添加样式：

```javascript
import React from "react";
import { View, Text } from "react-native";
import stylewind from "react-native-stylewind";

export default () => (
  <View style={[stylewind.flex, stylewind.items_center, stylewind.bg_white]}>
    <Text style={[stylewind.text_16, stylewind.text_blue]}>
      Hello, Stylewind!
    </Text>
  </View>
);
```

### **动态合并样式**

使用 `merge` 方法动态合并多个样式：

```javascript
import React from "react";
import { View, Text } from "react-native";
import { merge } from "react-native-stylewind";

export default () => (
  <View style={merge("flex items_center bg_white")}>
    <Text style={merge("text_16 text_blue")}>Hello, Stylewind!</Text>
  </View>
);
```
