# 关于JS
## ES6模块功能
- export 指定输出
  - 变量、函数
  - 可用as重命名：export v1 as method，将v1重命名为method
  - 可出现在模块任意位置，但需在模块顶层
- import 指定引入
  - 接受一对大括号
  - 不能改写接口
  - 具有提升效果，会被提升到头部，提前执行
  - import * as module1 from ''，整体加载
- export default
  - 为模块指定默认输出，使用者无需知道即将加载的模块有哪些属性和方法，此时其他模块在加载该模块时，可以任意指定名字，这是import后不需要{}
  - 一个模块只能有一个默认输出
  - 其实只是输出了一个名为default的变量
  - 可以用来输出类
- export和import的复合写法
  - 如果在一个模块之中，先输入后输出同一个模块，import语句可以与export语句写在一起
## 关于react
### 生命周期
- componentWillMount()
- componentDidMount()
- componentWillReceiveProps(nextProps)
- shouldComponentUpdate(nextProps,nextState)
- componentWillUpdate(nextProps,nextState)
- componentDidUpdate(preProps,preState)
- componentWillUnmount()
## 关于webpack
style-loader是将css-loader打包好的css代码以`<style>`标签的形式插入到html文件中
通过 webpack 配置项中的 use 指 定的 loader 是按照索引反向执行的
## 关于nodejs
- 连接路径：path.join([path1][, path2][, ...])
- 路径解析：path.resolve([from ...], to)，注意最后一个参数的传入，要是有.之类的符号，则是串联路径
- c
