
### 本文汇总了一些iOS上线审核时所遇到的问题，并总结相关问题的解决办法！

#### *《未完，待续！请点击Star持续关注最新动态！》* 

#### <span id="目录">目录：</span>

-------------------------------

1. [PLA-1.2审核案例](#PLA-1.2)

2. [Safety-1.2审核案例](#Safety-1.2)
 
3. [Performance-2.1审核案例](#Performance-2.1)
 
4. [2.3审核案例](#2.3)
 
5. [Performance-2.3.1审核案例](#Performance-2.3.1)

6. [2.3.10审核案例](#2.3.10)

7. [PLA-3.3.12审核案例](#PLA-3.3.12)
 
8. [PLA-3.3.2热更新审核案例](#PLA-3.3.2热更新审核案例)
 
9. [Legal-5.2.3审核案例](#Legal-5.2.3)

10. [Legal-5.3.3审核案例](#Legal-5.3.3)
 
11. [22.2审核案例](#22.2)

---------------------------------

#### 正文：

##### <span id="PLA-1.2">PLA-1.2审核案例</span> 

([目录](#目录))

__原因：__

用个人账户上传金融类应用。

理财、P2P等金融类相关产品的开发者们：目前，金融类应用只能用对应公司名称的开发者账号上传了。也就是说，如果用个人开发者账号提交金融类应用，会收到苹果的审核未过信息。

__附被拒理由原文:__

```
PLA1.2
The Seller and Artist names associated with your app do not reflect the name, "xxx有限责任公司," in the app or its name and metadata, as required by Section 1.2 of the Apple Developer Program License Agreement.（您的应用开发商名称和应用内/应用名称/关键词/描述中的名字（XXX有限责任公司）不匹配，违反了苹果开发者计划许可协议2.1。）
Next Steps
Your app must be published under a Seller name and Artist name that reflects the xxx有限责任公司 brand, If you have developed these apps on behalf of a client, please advise your client to add you to their development team of their developer account.（您的应用必须以符合XXX有限责任公司品牌名称的开发者账号上传。如果您是帮助客户开发的应用，请通知您的客户将您添加到他们的开发者账号团队成员中。）
您的应用必须以符合XXX有限责任公司品牌名称的开发者账号上传。如果您是帮助客户开发的应用，请通知您的客户将您添加到他们的开发者账号团队成员中。
```

##### <span id="Safety-1.2">Safety-1.2审核案例</span> 

([目录](#目录))

__原因：__

含UGC却未提供用户协议及举报功能。

如果应用内有发帖等UGC（用户产生内容）功能，但是却没有要求用户同意条款（EULA），也没有对敏感信息的举报措施等，也可能被拒。

__附被拒理由原文:__

```
Safety - 1.2
Your app enables the display of user-generated content but does not have the required precautions in place.
Next Steps
Please revise your app to implement all of the following precautions:
- Require that users agree to terms (EULA) and these terms must make it clear that there is no tolerance for objectionable content.
- A method for filtering objectionable content.
- A mechanism for users to flag objectionable content.
- The ability to block abusive users from the service.
- The developer must act on objectionable content reports within 24 hours by removing the content and ejecting the user who provided the offending content.
```

##### <span id="Performance-2.1">Performance-2.1审核案例</span> 

([目录](#目录))

__原因：__

应用出现崩溃、加载失败等非常明显的Bug。

2.1中明确指明：Make sure your app has been tested on-device for bugs and stability before you submit it……Please don’t treat App Review as a software testing service. We will reject incomplete app bundles and binaries that crash or exhibit obvious technical problems.（请确保你的应用在提交审核之前经过充分测试并且没有Bug……不要把应用程序审核当作软件测试服务，如果你的应用不完整或者存在明显的技术缺陷，它将直接被拒绝。）

__附被拒理由原文:__

```
Performance - 2.1
We discovered one or more bugs in your app when reviewed on Wi-Fi.
Specifically, when we attempt to log-in, an activity indicator would spin briefly, then dismisses itself with no further action taken by the app.
The user remains on the log-in screen, and is unable to use your app.
We've attached screenshot(s) for your reference.
Next Steps
Please run your app on a device to identify the issue(s), then revise and resubmit your app for review.
```

##### <span id="2.3">2.3审核案例</span> 

([目录](#目录))

__原因：__

应用描述、截图等与应用功能严重不符。

如果应用描述、截图和预览视频等营销/宣传性资料中介绍的功能与应用的实际功能大相径庭，或者苹果审核人员并没有在应用中发现应用描述或截图中展示的功能，都有可能被拒。
除此之外，截图太过艺术化，完全不符合应用的实际内容，或选择的分类和应用性质完全不符等等都有可能被拒。

__附被拒理由原文:__

```
2.3 Details
We were unable to locate some of the features described in your marketing materials or app name.
Specifically, we are unable to locate 'xxx ' features that marketed in the app name.
Next Steps
If these features are located in your app, please reply to this message in the Resolution Center to provide information on how to locate them.
Alternatively, please revise your app to ensure that these features are fully implemented or revise your application description, release notes and screenshots to remove this content.
```

##### <span id="Performance-2.3.1">Performance-2.3.1审核案例</span> 

([目录](#目录))

__原因：__

包含隐藏功能。

不要在应用中包含任何隐藏以及没有相关说明文档的功能。如果应用的功能不能让审核人员了解清楚，很可能被拒。且苹果在审核规则中还有这样一条规定：如果这样的行为过分或者反复出现，你可能会被从开发者身份当中除名。

__附被拒理由原文:__

```
Performance - 2.3.1
We noticed that your app contains hidden features.
Specifically, your app contains a hidden music downloader.
Next Steps
Please remove these features from your app.
```

##### <span id="2.3.10">2.3.10审核案例</span> 

([目录](#目录))

__原因：__

出现第三方移动平台的名字、图标等。

苹果应用商店审核指南2.3.10规定：Make sure your app is focused on the iOS, Mac, Apple TV or Apple Watch experience, and don’t include names, icons, or imagery of other mobile platforms in your app or metadata, unless there is specific, approved interactive functionality.（确保你的应用专注于iOS、Mac、Apple TV or Apple Watch,在应用或者元数据中不包含其他平台的名称、图标、图像，除非有特定的、被认可的互动功能。）
也就是说，最好不要在苹果的应用商店出现和Android等平台有有关的信息，否则被拒的风险大大的。

__附被拒理由原文:__

```
2.3.10
DetailsWe found that your app and/or its metadata contains inappropriate or irrelevant platform information, which is not in compliance with the App Store Review Guidelines.
Specifically, your app mentioned other platforms, such as Android.
Next Steps
Providing future platform compatibility plans, or other general platform references, is not appropriate in the context of the App Store. It would be appropriate to remove this information.
```

##### <span id="PLA-3.3.12">PLA-3.3.12审核案例</span> 

([目录](#目录))

__原因：__

采集了IDFA却未集成广告服务。

IDFA (identifier for advertising)能够较精准地识别用户，尤其对广告主追踪广告转化率帮助很大。苹果开发者计划许可协议中规定：只有使用广告服务才有权采集IDFA。

__附被拒理由原文:__

```
PLA 3.3.12
We found that your app uses the Advertising Identifier but does not include ad functionality. This does not comply with the terms of the Apple Developer Program License Agreement, as required by the App Store Review Guidelines.
Specifically, section 3.3.12 of the Apple Developer Program License Agreement states:
"You and Your Applications (and any third party with whom you have contracted to serve advertising) may use the Advertising Identifier, and any information obtained through the use of the Advertising Identifier, only for the purpose of serving advertising. If a user resets the Advertising Identifier, then You agree not to combine,correlate, link or otherwise associate, either directly or indirectly, the prior Advertising Identifier and any derived information with the reset Advertising Identifier."
```

##### <span id="PLA-3.3.2热更新审核案例">PLA-3.3.2热更新审核案例</span> 

([目录](#目录))

__原因：__

近期不少开发者APP中集成或SDK中包含了热更新功能,受到苹果警告。

目前已知的有高德地图、个推、BugTags、Bugly含有热更新功能。
如果你的应用里集成的有这些第三方的sdk，请移步到其相关的官网，查看是有最新的sdk，如果有那么请替换掉最新的sdk。或者咨询其相关的技术支持人员，或者在其论坛发帖询问解决办法。

__附被拒理由原文:__

```
Your app, extension, and/or linked framework appears to contain code designed explicitly with the capability to change your app’s behavior or functionality after App Review approval, which is not in compliance with section 3.3.2 of the Apple Developer Program License Agreement and App Store Review Guideline 2.5.2. This code, combined with a remote resource, can facilitate significant changes to your app’s behavior compared to when it was initially reviewed for the App Store. While you may not be using this functionality currently, it has the potential to load private frameworks, private methods, and enable future feature changes. 
This includes any code which passes arbitrary parameters to dynamic methods such as dlopen(), dlsym(), respondsToSelector:, performSelector:, method_exchangeImplementations(), and running remote scripts in order to change app behavior or call SPI, based on the contents of the downloaded script. Even if the remote resource is not intentionally malicious, it could easily be hijacked via a Man In The Middle (MiTM) attack, which can pose a serious security vulnerability to users of your app.
Please perform an in-depth review of your app and remove any code, frameworks, or SDKs that fall in line with the functionality described above before submitting the next update for your app for review.
Best regards
App store Review
```

##### <span id="Legal-5.2.3">Legal-5.2.3审核案例</span> 

([目录](#目录))

__原因：__

App Store审核条款里明确规定：

①不要使用受保护的第三方内容，如商标、版权作品，或者在应用中使用未经专利许可的创意。

②如果你的应用使用、访问、展示和商业化第三方的服务，请保证你已经获得了相应的授权许可，且必须根据要求在审核前一并提供许可文件。

③应用程序不能对非法分享、保存、转换或者来自第三方源的数据的非法使用提供方便，除非具有相应的合法授权协议。

除此之外，苹果也出台了一系列保护自身知识产权的条款，例如：

①不要明示或暗示苹果公司是你的应用的供应商，或者苹果为你的应用的功能和质量代言。

②禁止创建一个与苹果已有产品、用户界面、应用、广告主题相似的应用，且不允许拼错苹果产品名称。

__附被拒理由原文:__

```
Legal - 5.2.3
Your app also allows users to either save or download music and/or video content without authorization from the relevant third-party sources.
Next Steps
Please provide documentary evidence of your rights to allow music or video content download from their sources. If you do not have the requested permissions, please remove the music or video download functionality from your app.
```

##### <span id="Legal-5.3.3">Legal-5.3.3审核案例</span> 

([目录](#目录))

__原因：__

错误使用抽奖、竞猜等促销方式。

抽奖、彩票、竞猜等功能可能是应用使用最普遍的促销方式之一了，而苹果对这些也做出了规定。

例如：

①用于抽奖和竞猜的官方规则必须在应用当中予以提供，并且明确表明苹果公司不是赞助商或者以任何形式参与了该活动；

②应用不允许使用应用内付费购买信用点或者虚拟货币，并把它们与实际的货币结合使用，也不允许在应用当中购买彩票、抽奖券，和进行资金转移……如果你没有完全明白苹果对这方面的审核条款，很可能被拒！


__附被拒理由原文:__

```
Legal - 5.3.3
Your app enables users to purchase a raffle ticket, top-up their accounts or initiate fund transfers in the app, which does not comply with the App Store Review Guidelines.
Next Steps
While raffle tickets cannot be purchased within the app, you may provide a link that launches your web site, in Safari, and enables ticket purchase.
```

##### <span id="22.2">22.2审核案例</span> 

([目录](#目录))

__原因：__

包含虚假、误导用户的信息或功能
如果名称、描述等应用信息或功能中包含虚假、山寨的成分，被苹果认定为：有误导用户的嫌疑，审核时就会被拒绝。

__附被拒理由原文:__

```
22.2 Details
Your app or its metadata contains misleading content. Specifically, your app name, xxx, misleads users that the app includes ability to earn cash.
Next Steps
Please remove or revise any misleading content in your app and its metadata.
```


------------------------------------------------------

> #### *《未完，待续！请点击Star持续关注最新动态！》* 
