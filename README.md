# Yenai-Plugin-safefork

本仓库是[yenai-plugin](https://github.com/yeyang52/yenai-plugin)的一个fork，遵循GPLv3协议。

本仓库移除了源仓库中一些开发者为了保留最终控制权而加入的后门代码（将4位成员的QQ视为机器人主人）；  
**但是：** 本仓库不保证已经移除了所有后门代码，建议使用者仍需自行审查代码。

注意：使用者应当遵守与源仓库相同使用要求，包括不得用于非法用途、不得在国内平台上宣传本项目等。

## 使用方法

使用方法与源仓库相同，仅需：

**Github：**  
将`https://github.com/yeyang52/yenai-plugin` 替换为 `https://github.com/shing-yu/yenai-plugin`

**Gitee：**
将`https://gitee.com/yeyang52/yenai-plugin` 替换为 `https://gitee.com/xingyv1024/yenai-plugin`

**星隅的私有Git服务器（IPv6 only）：**
将`https://github.com/yeyang52/yenai-plugin` 替换为 `https://git.shingyu.cn:60/shingyu/yenai-plugin`

## 说明

我们理解源仓库开发者为了防止插件被滥用而加入了使自己能够控制插件的代码，但是我们认为这种做法是不负责任的。  
或者至少应该在插件的说明文档中明确提醒这一点，而不是在代码中通过各种方式隐藏这一事实。  
我们认为，如果代码中存在任何一个后门代码，那么将导致用户丧失对整个项目乃至其作者的信任，甚至可能导致用户对整个开源社区的产生质疑；我们认为这种做法得不偿失。  
我们承诺，如果源仓库开发者采取 移除后门/明确告知用户后门的存在以及遵守使用条件的约定 ，我们将立即存档本仓库。

源仓库后门隐藏方式：
在.github/ISSUE_TEMPLATE/中，存在一个没有文件名的序列化文件，其中包含了源开发者的QQ号MD5值；在代码中对其进行了反序列化并用于判断。
