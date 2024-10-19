[合集 \- 开源项目推荐(4\)](https://github.com)[1\.还在为找开源项目发愁么？或许这个项目能帮助你08\-02](https://github.com/xiezhr/p/18337904)[2\.金九银十来了，你的简历写好了么？09\-02](https://github.com/xiezhr/p/18392058)[3\.喜欢干净简洁音乐播放器的朋友看过来09\-10](https://github.com/xiezhr/p/18405717)4\.MiGPT让你的小爱音响更聪明10\-18收起
大家好，我是**晓凡**。


今天要给大家带来一个超级有趣的开源项目`MiGPT`。


这个项目，简直就是给小爱音箱装上了超级大脑，**让你的小爱音箱更聪明。**


想象一下，当小爱音箱接入大模型后，上知天文，下知地理，从“人工智障”秒变学霸。


### 一、什么是MiGPT



> `MiGPT`是一个由`idootop`团队开发的开源项目，目前已经获得了`7.5k`的Star，这在`GitHub`上可是相当受欢迎的。
> 
> 
> `MiGPT` 通过将小爱音箱、米家智能设备，与 `ChatGPT` 的理解能力完美融合，让你的智能家居更懂你。


① 开源地址


[https://github](https://github.com).**com**/idootop/mi\-gpt


![开源地址](https://img2024.cnblogs.com/blog/2381533/202410/2381533-20241018090752865-352025560.png)


②官方演示视频


视频地址：[https://www.ixigua.com/7426731715105653298](https://github.com)



### 二、MiGPT功能


* **🎓 AI 问答**。小爱音箱接入大模型后，上知天文，下知地理，从“人工智障”秒变学霸。
* **🎭 角色扮演**。一秒调教小爱，无论是成为你的完美伴侣，还是那个能听你倾诉心事的贴心闺蜜，都不在话下。
* **💬 流式响应**。爱情来得太快就像龙卷风，而你的小爱音箱也是，对你的爱意秒回，爱你不会让你等太久。
* **🧠 长短期记忆**。小爱音箱现在能记住你们之间的每一次对话，越聊越默契，就像是你身边的老朋友。
* **🔊 自定义 TTS**。厌倦了小爱同学的语音？帮你解锁[「豆包」](https://github.com)同款音色，就像真人在回你的消息。
* ~~**🤖️ 智能家居 Agent**。心情不好？小爱立刻懂你，自动帮你播放喜欢的音乐，调节灯光，逗你开心。~~


### 三、使用前准备


#### 3\.1 设备要求


`MiGPT` 支持大部分的小爱音箱型号，但对有些型号是不支持的。像小度音箱、天猫精灵、`HomePod` 等智能音箱设备。


大家在实用前一定要确认好自己的设备型号，以免出现一些不必要的麻烦。


下面例举出支持和不支持的设备供大家参考（数据来源于网络小伙伴）


* 可以完美运行的型号




| 名称 | 型号 | ttsCommand | wakeUpCommand | playingCommand | streamResponse | 反馈来源 |
| --- | --- | --- | --- | --- | --- | --- |
| 小爱音箱 Pro | [LX06](https://github.com) | `[5, 1]` | `[5, 3]` | \- | true | [@idootop](https://github.com) |
| 小爱音箱 mini | [LX01](https://github.com) | `[5, 1]` | `[5, 2]` | `[4, 1, 1]` | true | [@gsscsd](https://github.com) |
| 小爱音箱 Play（2019 款） | [LX05](https://github.com) | `[5, 1]` | `[5, 3]` | `[3, 1, 1]` | true | [@wt666666](https://github.com) |
| 小爱音箱 万能遥控版 | [LX5A](https://github.com) | `[5, 1]` | `[5, 3]` | \- | true | [@imhsz](https://github.com) |
| 小米 AI 音箱 | [S12](https://github.com) | `[5, 1]` | `[5, 3]` | \- | true | 微信: CMSJ |
| 小米 AI 音箱（第二代） | [L15A](https://github.com) | `[7, 3]` | `[7, 1]` | `[3, 1, 1]` | true | 微信: 龙之广 |
| 小爱智能家庭屏 10 | [X10A](https://github.com) | `[7, 3]` | `[7, 1]` | \- | true | [@IDarkBoss](https://github.com) |
| Xiaomi Sound Pro | [L17A](https://github.com) | `[7, 3]` | `[7, 1]` | \- | true | 微信: eof |


* 可以正常运行 `MiGPT`，但不支持连续对话的小爱音箱型号




| 名称 | 型号 | ttsCommand | wakeUpCommand | playingCommand | streamResponse | 反馈来源 |
| --- | --- | --- | --- | --- | --- | --- |
| 小爱音箱 | [L06A](https://github.com) | `[5, 1]` | `[5, 2]` | \- | false | [@zhanglc](https://github.com):[milou加速器](https://xinminxuehui.org) |
| 小爱音箱 Play | [L05B](https://github.com) | `[5, 3]` | `[5, 1]` | \- | false | [@BiuBiu2323](https://github.com) |
| 小米小爱音箱 Play 增强版 | [L05C](https://github.com) | `[5, 3]` | `[5, 1]` | \- | false | [@lyddias](https://github.com) |
| Xiaomi 智能家庭屏 6 | [X6A](https://github.com) | `[7, 3]` | `[7, 1]` | \- | false | [@Hongwing](https://github.com) |
| Redmi 小爱触屏音箱 Pro 8 英寸 | [X08E](https://github.com) | `[7, 3]` | `[7, 1]` | \- | false | [@shangjiyu](https://github.com) |
| 小爱音箱 Art | [L09A](https://github.com) | `[3, 1]` | `[3, 2]` | \- | false | [@zwsn](https://github.com) |
| 小爱触屏音箱 | [LX04](https://github.com) | `[5, 1]` | `[5, 2]` | \- | false | [@ilovesouthpark](https://github.com) |


* 完全不支持




| 名称 | 型号 | 反馈来源 |
| --- | --- | --- |
| 小米小爱音箱 HD | [SM4](https://github.com) | [@romantech](https://github.com) |
| 小米小爱蓝牙音箱随身版 | \- | 微信: 明天 |


#### 3\.2视频教程



> `MiGPT`作者很贴心，生怕大家不会运行，还自己录制了视频


视频地址：[https://www.bilibili.com/video/BV1zb421H7cS/?vd\_source\=1da677016e82657d6d824923c1d481a3](https://github.com)


### 四、怎么部署？


`MiGPT` 开源项目提供了两种部署方式，可以选择通过 `Docker` 或 `Node.js` 的方式部署。


对于不熟悉代码配置的用户，可以选择使用 `Docker` 进行快速部署。


对于有 `Node.js` 开发经验的用户，可通过 `npm` 安装相关依赖并运行项目


#### 4\.1 Docker部署


① 参数配置配置 `.migpt.js`


重命名本项目根目录下的 `.migpt.example.js`文件为 `.migpt.js`


![migpt.js配置](https://img2024.cnblogs.com/blog/2381533/202410/2381533-20241018090752816-1997927348.png)


详细参数参考：[https://github.com/idootop/mi\-gpt/blob/main/docs/settings.md](https://github.com)


②环境变量配置 `.env`


重命名本项目根目录下的 `.env.example` 文件为 `.env`。


![image-20241017200136784](https://img2024.cnblogs.com/blog/2381533/202410/2381533-20241018090752723-1820658036.png)


详细配置参考：[https://github.com/idootop/mi\-gpt/blob/main/docs/settings.md](https://github.com)


③ 启动 docker


以上配置好之后，按照如下命令启动`docker`



```


|  | docker run -d --env-file $(pwd)/.env -v $(pwd)/.migpt.js:/app/.migpt.js idootop/mi-gpt:latest |
| --- | --- |


```

#### 4\.2 Node.js 部署


① 安装依赖



```


|  | npm install mi-gpt # 安装依赖 |
| --- | --- |


```

② 参数配置于上面docke小节的一样



> 配置 `.migpt.js` 和 环境变量配置 `.env`


③ 启动 `MiGPT` 实例



```


|  | import { MiGPT } from "mi-gpt"; |
| --- | --- |
|  |  |
|  | async function main() { |
|  | const client = MiGPT.create({ |
|  | speaker: { |
|  | userId: "987654321", // 注意：不是手机号或邮箱，请在「个人信息」-「小米 ID」查看 |
|  | password: "123456", // 账号密码 |
|  | did: "小爱音箱Pro", // 小爱音箱 ID 或在米家中设置的名称 |
|  | }, |
|  | }); |
|  | await client.start(); |
|  | } |
|  |  |
|  | main(); |


```

#### 4\.3 使用


启动成功后，你可以通过以下方式来召唤 AI 回答问题：


* **小爱同学，请 xxx**。比如 `小爱同学，请问地球为什么是圆的？`
* **小爱同学，你 xxx**。比如 `小爱同学，你喜欢晓凡么？`
* **小爱同学，召唤 xxx**。比如 `小爱同学，召唤傻妞`


### 五、其他相关推荐


#### 5\.1 MiGPT GUI



> 通过图形化界面的方式创建并管理 MiGPT，支持运行多个账号


官网:[https://migptgui.com/](https://github.com)


![图形界面](https://img2024.cnblogs.com/blog/2381533/202410/2381533-20241018090752752-1645158181.png)


#### 5\.2 shinedlc/mi\-gpt



> 支持摄像头模块的 MiGPT 分支，让小爱同学可以看到和理解现实世界


项目地址：[https://github.com/shinedlc/mi\-gpt](https://github.com)


![image-20241017202114724](https://img2024.cnblogs.com/blog/2381533/202410/2381533-20241018090753098-767194198.png)


#### 5\.3 接入各种大模型



> 接入豆包、Moonshot（Kimi）、通义千问、质谱AI等大模型


具体教程参考：[https://migptgui.com/docs/apply/](https://github.com)


![接入各种大模型](https://img2024.cnblogs.com/blog/2381533/202410/2381533-20241018090752634-2058653858.png)


以上就是本期内容的全部，希望对您有所帮助。


大家觉得`MiGPT` 怎么样呢？欢迎评论区留言。


我们下期再见 ヾ(•ω•\`)o (●'◡'●)


