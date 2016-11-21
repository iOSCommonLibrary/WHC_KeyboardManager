WHC_KeyboradManager
==============
[![Pod License](http://img.shields.io/cocoapods/l/WHC_Model.svg?style=flat)](https://opensource.org/licenses/MIT)
简介
==============
- **高效**: 轻量级拒绝复杂或看不懂的Api
- **安全**: 拒绝监听干扰整个App,无入侵性,局部键盘监控处理
- **优势**: 集成简单设置灵活
- **简单**: 无需任何复杂配置
- **灵活**: 可自定义键盘处理配置
- **兼容**: 支持横竖屏切换适配
- **咨询**: 712641411
- **作者**: 吴海超

演示
==============
<img src = "https://github.com/netyouli/WHC_KeyboradManager/blob/master/WHC_KeyboradManager/demo/k1.gif", width = "375"><img src = "https://github.com/netyouli/WHC_KeyboradManager/blob/master/WHC_KeyboradManager/demo/k2.gif", width = "375">


要求
==============
* iOS 8.0 or later
* Xcode 8.0 or later

集成
==============
* 使用CocoaPods:
  -  pod 'WHC_KeyboradManager', '~> 1.0.0'
* 手工集成:
  -  导入文件夹WHC_KeyboradManager

用法
==============

- 无配置演示
```Swift
override func viewDidLoad() {
    super.viewDidLoad()
    /*******只需要在要处理键盘的界面创建WHC_KeyboradManager对象即可无需任何其他设置*******/
    WHC_KeyboradManager.share.addMonitorViewController(self)
}
```
- 自定义配置演示

```Swift
override func viewDidLoad() {
    super.viewDidLoad()
    /*******只需要在要处理键盘的界面创建WHC_KeyboradManager对象即可无需任何其他设置*******/
    let configuration = WHC_KeyboradManager.share.addMonitorViewController(self)
    /// 不要键盘头
    configuration.enableHeader = false

    /***configuration里面有丰富实用的自定义配置具体可参看代码***/
}
```

推荐
==============
- WHC_DataModelFactory mac工具github地址：https://github.com/netyouli/WHC_DataModelFactory

## <a id="期待"></a>期待

- 如果您在使用过程中有任何问题，欢迎issue me! 很乐意为您解答任何相关问题!
- 与其给我点star，不如向我狠狠地抛来一个BUG！
- 如果您想要更多的接口来自定义或者建议/意见，欢迎issue me！我会根据大家的需求提供更多的接口！

## Licenses
All source code is licensed under the MIT License.
