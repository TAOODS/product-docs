# 游戏礼包与福利活动

::: tip 阅读本文大概需要20分钟

本文主要从游戏活动、游戏福利的运营角度出发，对礼包、活动模版、福利配置等玩法进行讨论，也许能对您提高日活、留存、玩家体验有所帮助哦。

::: 
## 礼包管理

233乐园支持礼包功能，创作者可以自主新建礼包，系统将自动生成礼包兑换码。创作者中心礼包按照用途被分为了**活动礼包**和**福利礼包**，各自有礼包管理页面，提供创建礼包、查看礼包领取数量、补充库存、删除礼包等功能，对于审核中礼包也可撤回审核再编辑。另外创作者也可以在[【生成礼包码】](https://portal.ark.online/#/admin/prop-list-other "创作者中心-生成礼包码")页面只新建礼包并生成兑换码而不用于活动或福利。
![img](https://arkimg.ark.online/(null)-20241106154352994.png)
### 创建礼包

#### 1. 从礼包管理新增礼包
| **游戏活动-新增礼包**                                               | **福利礼包-新增礼包**                                               |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://qn-cdn.233leyuan.com/athena/online/f821b601a13f487b855036f5d5bef752_434302213.webp) | ![img](https://qn-cdn.233leyuan.com/athena/online/8789f3caf7734fb1a2145bfb5b3508f9_434302214.webp) |
- **礼包名称**：该字段会对外展示，建议取名简短有重点，填写礼包核心物品，体现礼包价值，可勾选“附上游戏名称”，方便玩家在管理礼包时明确礼包归属
> 提示：尽量保证在20字以内（不限制），如“《王者荣耀》签到7天礼包(皮肤碎片*20)"
- **礼包图标**：要求比例1：1，大小50KB内
- **礼包描述**：会对外展示，建议描述完整内容，如“xx游戏✖233乐园联名稀有钻石*10”
- **时长类型**：该字段指用户可使用这个礼包的时间段，过期后该礼包将不可见、不可用
> 提示：请根据活动需要合理设置礼包的时长类型：永久有效/固定时间段/领取后n小时内
- **礼包初始库存**：设置礼包初始数量，系统将生成对应数量的兑换码，一个礼包兑换码只能被兑换一次
- **礼包兑换规则**：不限次数：玩家拿到多个未被兑换的兑换码后就能兑换多次；仅可兑换一次：玩家只能兑换一次礼包，系统会校验玩家的领取记录，兑换过的玩家使用其他兑换码会提示兑换失败
- **礼包信息**：json格式，玩家兑换成功后向创作者发送回调，创作者可在此处自定义兑换成功的回调信息，可用于相关统计或其他代码逻辑
- **提审说明**：仅供审核人员查看，不会呈现给用户。建议标识出可兑换的游戏版本号、游戏内的兑换方式，以确保审核的及时性
- **预估价值**：填写该礼包价值多少元
#### 2. 创建活动/福利的同时新增礼包
以福利礼包为例，您也可以在创建活动或福利的过程中新建礼包，这与从礼包管理处新建礼包没有区别
| **新增福利**                                               | **点击新建礼包**                                               |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://qn-cdn.233leyuan.com/athena/online/5e2db947e14941f4ae08d7fd04bf3e14_434424456.webp) | ![img](https://qn-cdn.233leyuan.com/athena/online/3cac919eb64e4081aca6236f3a516ba6_434424457.webp) |

福利详情页和礼包详情页在233乐园的展示效果如下图所示：
| **福利详情页**                                               | **礼包详情页**                                               |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://arkimg.ark.online/(null)-20241106154353607.png) | ![img](https://arkimg.ark.online/(null)-20241106154352872.png) |
### 撤销审核/编辑/补充库存
1. 对于审核中礼包，如有问题可以点击操作列的【撤回审核】后，再次【编辑】后提交
2. 审核通过已投入福利/活动中使用的礼包，可以关注下【兑换/领取/总量】列，如库存不足，点击操作列的【补充库存】上传兑换码进行补充
3. 点击【记录】，可查看兑换码的生成记录以及玩家的兑换记录
## 游戏活动介绍

为帮助创作者更好的运营游戏活动、提高玩家活跃和留存，创作者中心提供了通用的H5活动模版，用于创作者直接配置运营活动、激励玩家完成任务发放奖励。
> 支持配置的活动类型：签到活动、抽奖任务活动、新游预约活动、新版本预约活动。

### 运营位
游戏活动支持放置的运营位包括公告、福利详情页、悬浮球等，您可以在创作者中心直接发布活动到[【运营公告】](https://portal.ark.online/#/admin/announcement-list)，并可提供资源位banner素材（尺寸要求详见下图）给乐园运营，由乐园运营帮您发布到对应资源位，如有特殊需求也可联系运营处理。

| **游戏公告**自行在[运营公告](https://portal.ark.online/#/admin/announcement-list)发布 | **福利详情页** 活动审核通过会自动同步  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://arkimg.ark.online/(null)-20241106165525323.png) | ![img](https://arkimg.ark.online/(null)-20241106165525864.png)|

以下资源位置需要您准备素材联系乐园运营发布

| **首页悬浮球**                | **游戏内悬浮球**              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://arkimg.ark.online/(null)-20241106165523489.png)| ![img](https://arkimg.ark.online/(null)-20241106165527367.png)|

### 活动类型

创建活动在[【游戏活动】](https://portal.ark.online/#/admin/active-template)配置页右上角点击新增按钮，选择要使用的活动模板类型后，填写相关素材信息并提交审核，即完成创建。以下是四种活动模版在233乐园的表现：
| **签到活动**                                                 | **抽奖活动**                                                 | 
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://arkimg.ark.online/(null)-20241106165522381.png) | ![img](https://arkimg.ark.online/(null)-20241106165523232.png) |

| **版本预约活动**                                                 | **新游预约活动**                                                 | 
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://qn-cdn.233leyuan.com/athena/online/056e3224d06746e88f125f7d302c6956_432391328.webp) | ![img](https://qn-cdn.233leyuan.com/athena/online/f2356130a0b2409a9af499aea41e9fd2_432391387.webp) |

### 签到活动

游戏签到活动是为了提高玩家活跃、留存设计的通用性活动，创作者可以设计用户奖励，在开发中平台的【游戏活动】页面配置签到活动模板。

#### 创建活动（签到）

| **素材内容** | **素材说明和要求**                                           |
| ------------ | ------------------------------------------------------------ |
| 活动名称     | 会直接展示在各个运营位，建议突出活动主题和奖励内容，吸引用户点进活动 |
| 活动开始时间 | 玩家可以开始参加活动的时间审核通过状态下，部分资源位会根据该时间展示到C端 |
| 活动结束时间 | 玩家结束参加活动的时间，玩家不能参加签到活动，但可以查看到活动内容 |
| 活动关闭时间 | 活动正式关闭的时间，部分资源位会根据该时间结束展示到C端      |
| 模板类型     | 选择【签到活动】                                             |
| 图片         | 模板的背景banner图片建议尺寸720*430，png或jpg，大小200kb以内底部建议以背景色做渐变过渡![img](https://arkimg.ark.online/(null)-20241106165525700.png) |
| 活动背景颜色 | 模板整体的背景色，建议和banner图片色系匹配                   |

#### 活动规则-签到奖励

| **素材内容**     | **素材说明和要求**                                           |
| ---------------- | ------------------------------------------------------------ |
| 活动背景颜色     | 模板整体的背景色，建议和banner图片色系匹配                   |
| 签到奖励要求天数 | 签到规则设计，这里是用户领取下方奖励所需的连续签到天数![img](https://arkimg.ark.online/(null)-20241106165523790.png) |
| 奖励道具         | 点击【新增礼包】按钮，新建礼包（或选择之前已创建好的游戏礼包或编辑选中的礼包）礼包的配置管理说明【[点击查看](#props)】![img](https://qn-cdn.233leyuan.com/athena/online/33e249f918c341939d8966077c9b4a2e_432397761.webp) |
| 奖励图标         | 自动关联使用道具icon，您也可以重新上传icon，展示给用户的奖励图标图片比例建议1：1                         |
| 活动说明         | 告诉用户本次活动的要求和基本信息，通常包括：【活动时间】:【参与对象】:【参与方式】:【中奖说明】:![img](https://arkimg.ark.online/(null)-20241106165524090.png) |
| 分享描述         | 分享到外部第三方平台（微信、QQ）时会展示分享标题与分享描述，分享标题默认展示活动名称，分享描述为下方展示的描述文案。建议体现核心主题和奖励，简短有吸引力![img](https://arkimg.ark.online/(null)-20241106165524126.png) |

### 抽奖任务活动

#### 创建活动（抽奖）

| **素材内容** | **素材说明和要求**                                           |
| ------------ | ------------------------------------------------------------ |
| 活动名称     | 会直接展示在各个运营位，建议突出活动主题和奖励内容，吸引用户点进活动 |
| 活动开始时间 | 玩家可以开始参加活动的时间审核通过状态下，部分资源位会根据该时间展示到C端 |
| 活动结束时间 | 玩家结束参加活动的时间，玩家不能参加抽奖活动，但可以查看到活动内容 |
| 活动关闭时间 | 活动正式关闭的时间，部分资源位会根据该时间结束展示到C端      |
| 模板类型     | 选择【抽奖任务活动】                                         |
| 图片         | 模板的背景banner图片建议尺寸720*430，png或jpg，大小200kb以内底部建议以背景色做渐变过渡![img](https://arkimg.ark.online/(null)-20241106165526179.png) |
| 活动背景颜色 | 模板整体的背景色，建议和banner图片色系匹配                   |

#### 活动规则-抽奖奖励

| **素材内容**     | **素材说明和要求**                                           |
| -------------------- | ------------------------------------------------------------ |
| 奖励类型             | 抽奖奖励的奖品类型，支持道具、实物、Q币、抽奖次数、谢谢参与![img](https://arkimg.ark.online/(null)-20241106165524396.png) |
| 奖励道具             | 奖励类型为道具/实物，则需选择对应的道具id                    |
| 奖励名称             | 展示给用户的奖励名称                                         |
| 奖励图标             | 选择兑换码或实物时自动关联icon，您也可以重新上传icon，展示给用户的奖励图标图片比例建议1：1                         |
| 每日允许发放最大份数 | 该奖励每天可以发放的最大份数，可结合游戏礼包创建的数量，综合考虑填写-1则为无限制 |
| 每个用户获取上限次数 | 每个用户可以获取该奖励的上限数量，决定了用户是否可以重复完成任务并领取奖励，根据不同的任务类型可进行不同设计，填写-1则为无限制 |
| 概率                 | 用户获取该奖励的概率目前抽奖支持配置8个奖励，8个奖励的概率和须为100% |
| 权重                 | 权重决定该奖励展示在抽奖转盘位置的先后顺序，越大则越靠前权重大小对抽奖转盘处奖励展示顺序的影响如右图所示![img](https://arkimg.ark.online/(null)-20241106165525088.png) |
| 允许广播数量         | 用户抽奖后会在抽奖页面轮播中奖者，以激励大家都来参加活动谢谢参与建议广播数量填0![img](https://arkimg.ark.online/(null)-20241106165525471.png) |
| 任务名称             | 展示给用户的任务名称，需要将任务描述的简短清晰例如“每日游戏时长达到30分钟”![img](https://arkimg.ark.online/(null)-20241106165524641.png) |
| 任务类型             | 目前支持7种任务类型，包括”签到、分享、累计充值奖励、每日充值奖励、累计游戏时长、每日游戏时长、帖子回复”，根据运营目标需要，选择对应任务即可 |
| 任务要求             | 不同任务类型对应不同的任务要求：签到：每日签到可得任务奖励/每日任务分享：每日分享活动可得任务奖励/每日任务累计充值奖励：在游戏内充值达到指定金额可得任务奖励/一次性任务每日充值奖励：每日在游戏内充值达到指定金额可得任务奖励/每日任务累计游戏时长：在游戏内游玩时长达到指定分钟数可得任务奖励/一次性任务每日游戏时长：每日在游戏内游玩时长达到指定分钟数可得任务奖励/每日任务帖子回复：回复指定帖子可得任务奖励，点击按钮将跳转至指定帖子/一次性任务 |
| 任务奖励类型         | 任务奖励的奖品类型，支持道具、抽奖次数道具需要在游戏礼包处创建 |
| 奖励道具             | 奖励类型为道具/实物时才需要填，点击【新增礼包】按钮，新建礼包（或选择之前已创建好的游戏礼包）礼包的配置管理说明【[点击查看](#props)】![img](https://qn-cdn.233leyuan.com/athena/online/937b336ad18d4d7bb947f0ca6b7152b6_432400032.webp) |
| 活动说明             | 告诉用户本次活动的要求和基本信息，通常包括：【活动时间】:【参与对象】:【参与方式】:【中奖说明】:![img](https://arkimg.ark.online/(null)-20241106165525636.png) |
| 分享描述             | 分享到外部第三方平台（微信、QQ）时会展示分享标题与分享描述，分享标题默认展示活动名称，分享描述为下方展示的描述文案。建议体现核心主题和奖励，简短有吸引力![img](https://arkimg.ark.online/(null)-20241106165525539.png) |

### 预约活动

新游和版本预约活动的配置素材是一样的，不同点是新游预约活动不包含游戏下载模块、支持还没上架过乐园的游戏，版本预约活动包含游戏下载模块、只支持已经上架过的游戏

#### 创建活动（预约）

| **素材内容**     | **素材说明和要求**                                           |
| ------------ | ------------------------------------------------------------ |
| 活动名称     | 会直接展示在各个运营位，建议突出活动主题和奖励内容，吸引用户点进活动 |
| 活动开始时间 | 玩家可以开始参加活动的时间审核通过状态下，部分资源位会根据该时间展示到C端 |
| 活动结束时间 | 玩家结束参加活动的时间，玩家不能参加预约活动，但可以查看到活动内容 |
| 活动关闭时间 | 活动正式关闭的时间，部分资源位会根据该时间结束展示到C端      |
| 模板类型     | 选择【新游/版本预约活动】                                    |
| 图片         | 模板的背景banner图片建议尺寸720*430，png或jpg，大小200kb以内底部建议以背景色做渐变过渡 |
| 活动背景颜色 | 模板整体的背景色，建议和banner图片色系匹配                   |

#### 活动规则-预约奖励

| **素材内容**     | **素材说明和要求**                                           |
| ------------ | ------------------------------------------------------------ |
| 预约版本号   | 填写给用户预约的版本号如右图例填写的版本号为“新”![img](https://arkimg.ark.online/(null)-20241106165526145.png) |
| 上线日期     | 填写所预约版本上线的日期如右图例填写的日期为“11月13日0点”    |
| 自定义文案   | 选填，此处如果填写内容，将会优先展示此处填写的文案，隐藏版本号和上线日期。适用于一些有特殊文案需求的预约活动![img](https://arkimg.ark.online/(null)-20241106165526048.png) |
| 奖励类型     | 支持兑换码道具和游戏内道具兑换码道具：点击【新增礼包】新建礼包（或选择之前已创建好的游戏礼包）礼包的配置管理说明【[点击查看](https://doc.233leyuan.com/operate/game_activity.html#%E7%A4%BC%E5%8C%85%E9%85%8D%E7%BD%AE)】，平台根据预约情况发放兑换码给用户游戏内道具：由游戏方在游戏内发放给用户奖励，需要在活动说明里告知用户领取的规则 |
| 奖励条件类型 | 仅奖励类型为兑换码道具时需要填写，支持指定时间段领取或用户下载游戏后即可领取指定时间段领取需注意：时间段需要在活动的开始-关闭时间段内，保证本页面是上线状态，用户可以领取奖励 |
| 福利名称     | 填写福利名称，简单描述即可![img](https://arkimg.ark.online/(null)-20241106165525706.png) |
| 福利描述     | 填写福利里包含的具体内容，比如“稀有币*2，手套*1”             |
| 福利图片     | 要求图片比例1：1，50KB以内                                   |
| 活动说明     | 告诉用户本次活动的要求和基本信息，通常包括：【活动时间】:【参与对象】:【参与方式】:【中奖说明】:![img](https://arkimg.ark.online/(null)-20241106165525969.png) |
| 分享描述     | 分享到外部第三方平台（微信、QQ）时会展示分享标题与分享描述，分享标题默认展示活动名称，分享描述为本内容框填写的文案建议体现核心主题和奖励，简短有吸引力![img](https://arkimg.ark.online/(null)-20241106165526758.png) |
| 版本预告说明 | 选填，常用于说明本次版本上线/更新的核心玩法![img](https://arkimg.ark.online/(null)-20241106165526200.png) |
| 宣传描述     | 对宣传图片/视频内容的概括说明![img](https://arkimg.ark.online/(null)-20241106165526474.png) |
| 图片/视频    | 1280px × 720px                                               |

### 活动修改/复制

1. 对于未提审/已撤回审核的活动，可以点击操作区域 的【修改配置】对活动内容进行修改，点击【修改上线时间】对活动时间进行修改
2. 支持复制，点击想复制活动的操作区域 的【复制】可以复制出一个一模一样的活动，复制出的活动为待提审初始状态，可进行配置修改
3. 导出url，支持查看活动模版的H5链接，可复制后配置在公告或者在浏览器查看
![img](https://qn-cdn.233leyuan.com/athena/online/3b9d0b8ed5e646a694ac1772f66fcc97_434584951.webp)

## 福利礼包指南
福利礼包用于奖励【下载本游戏】的用户，从而激励用户下载本游戏、提高游戏曝光转化率。
> 福利礼包审核通过后会按上线时间展示在乐园游戏详情页的福利tab内，在库存足够情况下，每个用户都能点击按钮领取。

### 创建福利

首次进入福利礼包页面时，需要【单击创建】为游戏创建福利详情页
![img](https://qn-cdn.233leyuan.com/athena/online/a245a4ab7c6b486b82a82e455cb04559_434589512.webp)

创建福利在【福利礼包】页右上角点击新增按钮，填写相关展示要求信息后提交审核，即完成创建
![img](https://qn-cdn.233leyuan.com/athena/online/a7db9c49e16241a6be8c1d6f9d11c71d_434595783.webp)

###  **素材&配置指南**
福利详情页和礼包详情页在233乐园的展示效果如下图所示：
| **福利详情页**                                               | **礼包详情页**                                               |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![img](https://arkimg.ark.online/(null)-20241106154353566.png) | ![img](https://arkimg.ark.online/(null)-20241106154353003.png) |

- **关联礼包**：选择或编辑要展示的礼包，也可以点击【新增礼包】按钮直接新增礼包关联
- **福利开始时间**：该福利上线并展示到福利详情页的时间，从该时间开始用户可以领取福利
- **福利结束时间**：该福利下线时间，但仍会展示在福利详情页，从该时间开始用户不能点击领取福利
- **福利关闭时间**：该福利从福利详情页关闭的时间
> 福利的时间会自动关联礼包的有效时间，您也可以自行修改
- **展示图标**：自动使用礼包icon
- **使用方法简要介绍**：建议简要介绍礼包的兑换步骤
- **审核通过后自动上线**：
  - 默认选择“是”，审核通过后会按时间自动上线；
  - 如果选择“否”，审核通过需要手动拖动卡片上线

### 调整福利布局

1. 左侧预览福利展示的样式
2. 已上线福利栏，点击各个福利卡片可拖动调整福利顺序，调整后需点击右上角进行保存
3. 乐园运营有时会在我们内部后台为各游戏创建福利，CP可随意调整顺序

![img](https://qn-cdn.233leyuan.com/athena/online/83be500a5f674efbb8380c15bb1e89f7_434599827.webp)
