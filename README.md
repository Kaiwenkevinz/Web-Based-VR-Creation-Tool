# Web-Based-VR-Creation-Tool

## Demo
![image](picture or gif url)
## 如何使用 Yjs 获得实时数据？
监听 web socket + 监听 Yjs Shared Types

## 使用树形结构前，如何获取最新值并渲染？

组件 A 监听字符串 A -> 用户更新字符串 -> 回调中获取字符串 A 最新值 -> 调用相应的 setState  
组件 B 监听字符串 B -> 用户更新字符串 -> 回调中获取字符串 B 最新值 -> 调用相应的 setState  
组件 C 监听字符串 C -> 用户更新字符串 -> 回调中获取字符串 C 最新值 -> 调用相应的 setState  

### 如果需要新增组件 D，用来显示字符串 D，该怎么做？
创建组件 D，创建字符串 D，在组件 D 中监听



## 使用树形结构后，如何获取最新值并渲染？
![image](https://github.com/Kaiwenkevinz/Web-Based-VR-Creation-Tool-Demo/blob/main/imgs/after_tree.png?raw=true)
监听根节点 -> 用户更新字符串 -> 监听回调得到最新的树，树中包含了刚刚更新的字符串 -> 调用 setState，传入 JSON 化的树

子组件只需更新树节点