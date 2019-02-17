为了减少游戏内玩家聊天时的前缀长度，服务器采用了一些不同颜色的标签并按照格式 `<[位置1][位置2]位置3> 聊天内容` 显示。下面是标签列表和介绍

| 标签         | 位置 | 颜色                                       | 意义                                             |
|--------------|------|-------------------------------------------|--------------------------------------------------|
| [M]          | 1    | <span class ="minecraft-text-2">§2</span> | 主世界                                           |
| [N]          | 1    | <span class ="minecraft-text-c">§c</span> | 下界                                             |
| [E]          | 1    | <span class ="minecraft-text-e">§e</span> | 末路之地                                         |
| [R]          | 1    | <span class ="minecraft-text-a">§a</span> | 资源世界                                         |
| [#]          | 1    | <span class ="minecraft-text-9">§9</span> | Discord消息                                      |
| [Admin]      | 2    | <span class ="minecraft-text-c">§c</span> | 总管理员，标签有可能会被自定义。                   |
| [Builder]    | 2    | <span class ="minecraft-text-e">§e</span> | 建筑师，标签有可能会被自定义。                     |
| [Mod]        | 2    | <span class ="minecraft-text-6">§6</span> | 管理员，标签有可能会被自定义。                   |
|              | 2    | <span class ="minecraft-text-b">§b</span> | 捐款者，标签内容会被自定义或者根据所在用户组显示 |
| [Player]     | 2    | <span class ="minecraft-text-a">§a</span> | 玩家                                             |
| [Unverified] | 2    | <span class ="minecraft-text-9">§9</span> | 未验证的Discord用户                               |
|              | 3    | <span class ="minecraft-text-b">§b</span> | 管理团队                                         |
|              | 3    | <span class ="minecraft-text-6">§6</span> | 建筑团队                                         |
|              | 3    | <span class ="minecraft-text-2">§2</span> | 玩家                                             |
|              | 3    | <span class ="minecraft-text-3">§3</span> | Discord用户                                     |

简单来说，位置1是玩家当时所在的世界，位置2是玩家的用户组，位置3是玩家在服务器所担当的角色。


## 举个例子
### 一般情况
<ul class="bg-dark list-unstyled minecraft-text p-1">
    <li>&lt;<span class ="minecraft-text-2">[M]</span><span class ="minecraft-text-c">[Admin]</span><span class ="minecraft-text-b">Soniji</span>&gt; Meow</li>
    <li>&lt;<span class ="minecraft-text-c">[N]</span><span class ="minecraft-text-6">[Mod]</span><span class ="minecraft-text-b">Whitebai_</span>&gt; Hi</li>
    <li>&lt;<span class ="minecraft-text-e">[E]</span><span class ="minecraft-text-a">[Player]</span><span class ="minecraft-text-2">Dinnerbone</span>&gt; 🙃</li>
    <li>&lt;<span class ="minecraft-text-a">[R]</span><span class ="minecraft-text-e">[Builder]</span><span class ="minecraft-text-6">bk_owenk</span>&gt; Build!</li>
    <li><span class ="minecraft-text-7">&lt;<span class ="minecraft-text-9">[#]</span><span class ="minecraft-text-8">[Unverified]</span><span class ="minecraft-text-3">some one</span>&gt; SPAM! I mean musubi..</span></li>
    <li>&lt;<span class ="minecraft-text-9">[#]</span><span class ="minecraft-text-c">[Admin]</span><span class ="minecraft-text-3">Soniji</span>&gt; hmm...</li>
</ul>
上面的聊天记录按顺序意思为
- 一只在主世界的总管理员Soniji叫了一声Meow
- 在地狱的管理员Whitebai_说了一声Hi
- 一只在末路之地的Dinnerbone发了一个反转的Emoji
- 建筑师bk_owenk在资源世界说了一声Build!
- 一个Discord账户未关联到Minecraft账户的some one从Discord发了一句「SPAM! I mean musubi..」
- 总管理员Soniji从Discord发了一句「hmm...」

### 多重用户组
用户是可以同时存在于多个用户组的。显示规则为：
- 管理组用户名颜色（第3位置）永远显示为青色 (<span class ="minecraft-text-b">§b</span>)
- 没有建筑组以外的用户用户名颜色（第3位置）会显示为蓝色 (<span class ="minecraft-text-6">§6</span>)
- 玩家组用户名颜色（第3位置）永远显示为绿色 (<span class ="minecraft-text-2">§2</span>)
- 管理组第2位置不显示捐款者颜色
- 建筑师(Builder)与管理员(Mod)共存时，第二位置优先显示建筑师(Builder)
- 建筑师(Builder)与总管理员(Admin)共存时，第二位置优先显示总管理员(Admin) （因总管理员(Admin)已有建筑师(Builder)权限）

下面是一些例子:
<ul class="bg-dark list-unstyled minecraft-text p-1">
    <li>&lt;<span class ="minecraft-text-2">[M]</span><span class ="minecraft-text-3">[Builder]</span><span class ="minecraft-text-b">Soniji</span>&gt; Builder and Mod</li>
    <li>&lt;<span class ="minecraft-text-e">[E]</span><span class ="minecraft-text-3">[I Am Cat]</span><span class ="minecraft-text-b">Soniji</span>&gt; Customized Builder and Mod</li>
    <li>&lt;<span class ="minecraft-text-e">[E]</span><span class ="minecraft-text-6">[I Am Cat]</span><span class ="minecraft-text-b">Soniji</span>&gt; Customized Mod</li>
    <li>&lt;<span class ="minecraft-text-c">[N]</span><span class ="minecraft-text-b">[Player]</span><span class ="minecraft-text-2">Soniji</span>&gt; Sponser</li>
    <li>&lt;<span class ="minecraft-text-a">[R]</span><span class ="minecraft-text-b">[I am Cat]</span><span class ="minecraft-text-2">Soniji</span>&gt; Customized Sponser</li>
    <li>&lt;<span class ="minecraft-text-2">[M]</span><span class ="minecraft-text-b">[Builder]</span><span class ="minecraft-text-6">Soniji</span>&gt; Builder and Sponser</li>
    <li>&lt;<span class ="minecraft-text-2">[M]</span><span class ="minecraft-text-b">[I am Cat]</span><span class ="minecraft-text-6">Soniji</span>&gt; Customized Builder and Sponser</li>
</ul>
对应用户组为（这个部分跳过对所在世界的解释）
- 建筑师和管理员
- 建筑师，管理员，捐款者（因只有捐款者可自定义前缀）
- 管理员和捐款者（因只有捐款者可自定义前缀）
- 捐款者和玩家
- 捐款者和玩家
- 捐款者和建筑师
- 捐款者和建筑师
