# JOKER-Personal
unity游戏仓库
OnValidate() 会自动在执行时纠正数值
OnValidate()在Awake之前调用，所以它比Awake更早"知道"数值

事件是委托的解决方法，因为委托是可以在其他类里对委托进行订阅与调用的，而事件只能在本类里
订阅与调用，提高委托的安全性。
委托可以看成一个枚举，里面装函数的枚举。

1，Unity客户端注册登录相关：
支付宝登录使用的：客户端的 深度链接返回给服务器端，可以从服务器的页面跳转到游戏里



2，Unity技术transform相关：
 transform.Translate(Vector3.forward * distance, Space.Self);默认本地坐标为准移动Space.Self可改world.self
 transform.position+=Vector3.forward * distance；默认世界坐标为准移动


3,脚本核心思想，如果外界想改变对象的属性，那么对象可以在自己的脚本上创建公共函数来向外公开改变属性。
