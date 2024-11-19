# uBlockOrigin & uBlacklist 大型AI屏蔽列表

这是一个包含超过1000个网站的大型屏蔽列表，专门用于屏蔽包含AI生成内容的网站。可以结合uBlock Origin或uBlacklist使用，帮助清理搜索引擎（Google、DuckDuckGo和Bing）中的图片结果。

同时，也提供了适用于pihole和adguard的hosts文件。

### 重要提示：
目前请优先使用 [uBlacklist](#如何在uBlacklist中安装屏蔽列表)，而不是uBlock Origin。因为需要对uBlock Origin中的DOM目标进行一些重构，你也可以尝试使用uBlock，但可能效果不理想...

## 在uBlock Origin中安装屏蔽列表

### 一键导入过滤器

如果你已经安装了uBlock Origin，可以点击[这个链接](https://subscribe.adblockplus.org?location=https%3A%2F%2Fraw.githubusercontent.com%2Flaylavish%2FuBlockOrigin-HUGE-AI-Blocklist%2Fmain%2Flist.txt&title=Sites%20using%20AI%20generated%20content) 进行一键导入，操作简单快捷。

### 手动导入

1. 确保你已经安装了uBlock Origin扩展，支持的浏览器包括 [Firefox](https://addons.mozilla.org/zh-CN/firefox/addon/ublock-origin/)、[Chrome](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm) 或其他支持uBO的浏览器（包括Android上的Firefox）。
  
2. 点击uBlock Origin扩展图标，点击右下角的齿轮图标，进入控制面板。

3. 在控制面板中，点击顶部的“过滤列表”选项。

4. 向下找到并展开```导入```按钮。

5. 将以下URL复制粘贴到弹出的对话框中：
```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/list.txt
```

6. 应用更改，这样就设置完成了！

我们还提供了一个如何操作的视频教程：[视频教程链接](https://github.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/assets/128162304/7b8810dc-ce87-4cdc-8b5a-95dc5b0f56c3)

uBlock Origin会每天自动更新过滤列表，确保你始终拥有最新的过滤器。如果需要手动更新，只需点击新添加列表旁的秒表图标，再按下```立即更新```即可。

## 在uBlacklist中安装屏蔽列表

### 一键导入过滤器（仅支持Chrome浏览器，Firefox暂不支持）

如果你使用Chrome浏览器并已安装[uBlacklist](https://chrome.google.com/webstore/detail/ublacklist/pncfbmialoiaghdehhbnbhkkgmjanfhe)，可以点击[这个链接](https://iorate.github.io/ublacklist/subscribe?name=Main+AI+Blocklist&url=https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/list_uBlacklist.txt) 一键订阅屏蔽列表。

### 手动导入

1. 确保你已经安装了uBlacklist扩展，支持的浏览器包括 [Firefox](https://addons.mozilla.org/zh-CN/firefox/addon/ublacklist/)、[Chrome](https://chrome.google.com/webstore/detail/ublacklist/pncfbmialoiaghdehhbnbhkkgmjanfhe)或其他支持uBlacklist的浏览器（包括Android上的Firefox）。

2. 点击扩展列表，选择uBlacklist，然后点击蓝色的“选项”按钮。

3. 启用**其他搜索引擎**选项，并选择你希望屏蔽列表生效的搜索引擎。兼容的搜索引擎列表可在[这里查看](https://github.com/iorate/ublacklist?tab=readme-ov-file#supported-search-engines)。

4. 向下滚动到“订阅”标签，点击蓝色的“添加订阅”按钮。

5. 给添加的屏蔽列表起一个名字（例如：主AI屏蔽列表）。

6. 将以下URL复制粘贴到**URL**部分：
```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/list_uBlacklist.txt
```

7. 设置更新频率为每小时，以实现近乎实时的列表更新，完成后即可。

### iOS与iPadOS（Safari浏览器）

1. 从[App Store](https://apps.apple.com/us/app/ublacklist-for-safari/id1547912640)下载uBlacklist。

2. 打开设置，找到Safari并点击。

3. 在Safari设置中，点击**扩展**，然后启用uBlacklist扩展。

4. 在uBlacklist的设置中，找到**uBlacklist的权限**部分，设置搜索引擎的权限为“允许”。

5. 返回顶部，点击蓝色的**扩展设置**按钮，会自动打开Safari并显示uBlacklist的设置面板。

6. 向下滚动至“订阅”标签，点击蓝色的“添加订阅”按钮。

7. 为屏蔽列表命名（如：主AI屏蔽列表）。

8. 将以下URL复制粘贴到**URL**部分：
```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/list_uBlacklist.txt
```

9. 设置更新频率为每小时，完成。

## Pi-hole/AdGuard的Hosts文件

我们还提供了一个适用于Pi-hole或AdGuard的HOSTS格式列表，适用于操作系统的hosts文件中。

```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/noai_hosts.txt
```

访问此URL后，将内容复制粘贴到操作系统的hosts文件中即可，如何访问hosts文件的教程可见[这里](https://linuxize.com/post/how-to-edit-your-hosts-file/)。

### Pi-hole设置：
1. 访问Pi-hole管理面板。
2. 点击“广告列表”。
3. 将URL粘贴到“地址”框中。
4. 点击“添加”按钮。

### AdGuard设置：

1. 打开AdGuard Home面板。
2. 前往过滤器 --> DNS黑名单。
3. 点击“添加黑名单”，然后选择“添加自定义列表”。
4. 输入列表名称（如：AI屏蔽列表）。
5. 粘贴URL到第二个对话框中。
6. 点击保存即可。

## 屏蔽列表不起作用怎么办？

如果新导入的屏蔽列表不起作用，可能是因为浏览器的会话过期。可以尝试关闭**所有**浏览器窗口，等待4-5秒直至所有进程结束，然后重新打开浏览器。如果这样还是不行，可以尝试清除浏览器缓存。

## 其他屏蔽列表

目前有两个屏蔽列表：主列表和核选列表。

核选列表中包含了一些既有真实内容又有AI生成内容的网站（如DeviantArt、Artstation、图片库等），这些网站不适合直接屏蔽在主过滤列表中，所以将它们放到了单独的可选列表中。

### uBlock Origin
使用**核选**列表的方法和使用主列表的方法一样，只需要将URL替换为：

```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/additional_list_nuclear.txt
```

### uBlacklist
使用**核选**列表的方法和使用主列表的方法一样，只需要将URL替换为：

```
https://raw.githubusercontent.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist/main/list_uBlacklist_nuclear.txt
```

## 网站允许列表

不想屏蔽某些网站？可以通过uBlock Origin或uBlacklist来创建允许列表。

### uBlock Origin：
1. 通过uBlock Origin的[日志记录器](https://github.com/gorhill/uBlock/wiki/The-logger)，打开[DOM检测器](https://github.com/gorhill/uBlock/wiki/DOM-inspector)。
2. 找到你想允许的网站的URL。
3. 点击需要禁用的过滤器（例如：vecteezy.com），使其被划掉。
4. 保存更改并点击“创建”按钮。

或者，直接在过滤列表中添加以下行：
```
#@#a[href*="example.com"]:upward(div):style(opacity:0.00!important;)
```

将“example.com”替换为你想允许的网站地址，然后粘贴到uBlock Origin的“我的过滤器”中。

### uBlacklist：
1. 进入uBlacklist的选项面板。
2. 在文本框中添加以下行：
```
@*://*.example.com/*
```
3. 将“example.com”替换为你想允许的网站。
4. 点击保存即可。

## 扩展过滤功能

你可以根据关键词来屏蔽AI结果。这个功能原来包含在列表中，现在被移除了以便用户可选配置。

### uBlock Origin
你可以使用以下模板在你的个人过滤列表中添加自定义关键词：
```
google.com,duckduckgo.com,bing.com##div>a:has-text(/Your Text Here/i):upward(div):style(opacity:0!important)
```
将“Your Text Here”替换为你想屏蔽的关键词。以下是一些**可选**的过滤模板：
```
google.com,duckduckgo.com,bing.com##div>a:has-text(/Stable Diffusion/i):upward(div):style(opacity:0!important)
google.com,duckduckgo.com,bing.com##div>a:has-text(/AI Art/i):upward(div):style(opacity:0!important)
...
```

### uBlacklist

对于uBlacklist，可以使用[正则表达式](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Guide/Regular_Expressions)来根据关键词进行过滤，例如：
```
/ai *(generated)?|stable *diffusion/i
```

以下是一些**可选**的正则表达式，用于屏蔽AI内容：
```
/(generative)? *AI *(art|generated|illustration)?/i
...
```

## uBlock Origin与uBlacklist的区别

目前，uBlacklist在Google图片搜索分页上有一些问题，如果某页AI图片被屏蔽过多，可能无法加载更多内容。这种情况较少见，但确实存在。

而uBlock Origin不会有这个问题，因为它只是改变了div的透明度，并没有完全屏蔽元素，这意味着图片搜索中会有“空白”的位置。

如果uBlock Origin不起作用，可以尝试uBlacklist，反之亦然。可以分别试试，看哪个更适合你。

## 待办事项
✅ 提供与uBlacklist兼容的屏蔽列表

✅ 屏蔽DuckDuckGo和Bing的AI内容

✅ 创建适用于pi-hole/adguard的hosts文件

❌ 支持Startpage、Ecosia、Brave（uBlock Origin版）

## 特别感谢

+ 感谢这份[pastebin](https://pastebin.com/B8kP4imQ)，添加了更多的网站到我的屏蔽列表。
+ u/AchernarB 提供的[代码片段](https://www.reddit.com/r/uBlockOrigin/comments/13uyex5/how_to_block_results_from_a_specific_site_in_the/)。
+ Raymond Hill，uBlock Origin扩展作者。
+ iorate，uBlacklist扩展作者。

## 相关项目

[Super SEO Spam Suppressor (SSSS)](https://github.com/NotaInutilis/Super-SEO-Spam-Suppressor) - 一款针对利用SEO策略滥用网络的内容农场、抄袭者、AI生成内容等垃圾网站的封锁列表，适用于uBlacklist。

[Journey Buster 3](https://journeybuster.com/) - 一个可以识别Twitter上的AI生成图片的Chromium扩展。

[Awesome List of uBlacklist Subscriptions](https://github.com/rjaus/awesome-ublacklist) - 包含各种优秀的uBlacklist订阅列表。

[Anti-AI Google Search Tips](https://github.com/laylavish/TipsTricksGoogleSearch) - 提供在Google搜索中避免AI内容的技巧和建议。