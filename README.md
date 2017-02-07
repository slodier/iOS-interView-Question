无意中看到的面试题,有模棱两可的,想来还是记录下来,留着 free time 作提高,及日后查询之便利
=======
##吾日三省吾身
[1-1. 最近这两天你有学到什么知识/技能么?](#1)<br>
[1-2.  最近有做过比较酷或者比较有挑战的项目么?](#2)<br>
[1-3.  最近看过的书/文章有哪些?](#3)<br>
[1-4.  熟悉 CocoaPods 么? 能大概讲一下工作原理么?](#4)<br>
[1-5.  最常用的版本控制工具是什么,能大概讲讲原理么?](#5)<br>
[1-6.  今年你最想掌握的一门技术是什么? 为什么? 目前已经做到了哪个程度?](#6)<br>
[1-7.  你一般是怎么用 Instruments 的?](#7)<br>
[1-8.  你一般是如何调试 Bug 的?](#8)<br>
[1-9.  你在你的项目中用到了哪些设计模式?](#9)<br>
[1-10. 如何实现单例,单例会有什么弊端?](#10)<br>
[1-11. iOS 是如何管理内存的?](#11)<br>

##知识性问题
[2-1. 什么是响应链,它是怎么工作的?](#21)<br>
[2-2. 如何访问并修改一个类的私有属性?](#22)<br>
[2-3. iOS Extension 是什么? 能列举几个常用他的 Extension?](#23)<br>
[2-4. 如何把一个包含自定义对象的数组序列化到磁盘?](#24)<br>
[2-5. Apple Pay 是什么？它的大概工作流程是怎样的?](#25)<br>
[2-6. iOS 的沙盒目录结构是怎样的? App Bundle 里面都有什么?](#26)<br>
[2-7. iOS 的签名机制大概是怎样的?](#27)<br>
[2-8. iOS 7的多任务添加了哪两个新的 API? 各自的使用场景是什么?](#28)<br>
[2-9. Objective-C 的 class 是如何实现的？Selector 是如何被转化为 C 语言的函数调用的?](#29)<br>
[2-10. UIScrollView 大概是如何实现的,它是如何捕捉、响应手势的?](#210)<br>
[2-11. Objective-C 如何对已有的方法,添加自己的功能代码以实现类似记录日志这样的功能?](#211)<br>
[2-12. +load 和 +initialize 的区别是什么?](#212)<br>
[2-13. 如何让 Category 支持属性?](#213)<br>
[2-14. NSOperation 相比于 GCD 有哪些优势?](#214)<br>
[2-15. strong / weak / unsafe_unretained 的区别?](#215)<br>
[2-16. 如何为 Class 定义一个对外只读对内可读写的属性?](#216)<br>
[2-17. Objective-C 中,meta-class 指的是什么?](#217)<br>
[2-18. UIView 和 CALayer 之间的关系?](#218)<br>
[2-19. +[UIView animateWithDuration: animations: completion:] 内部大概是如何实现的?](#219)<br>
[2-20. @property (copy) NSMutableArray *array; 这个写法会出什么问题?](#220)<br>
[2-21. const 和 define 的区别?](#221)<br>
[2-22. 讲述一下 runtime 的概念, message send 如果寻找不到相应的对象,会如何进行后续处理?](#222)

##经验类问题
[3-1. 为什么 UIScrollView 的滚动会导致 NSTimer 失效?](#31)<br>
[3-2. 什么当 Core Animation 完成时,layer 又会恢复到原先的状态?](#32)<br>
[3-3. 你会如何存储用户的一些敏感信息,如登录的 token.](#33)<br>
[3-4. 有用过一些开源组件吧,能简单说几个么,大概说说它们的使用场景实现.](#34)<br>
[3-5. 什么时候会发生 EXC BAD ACCESS 异常?](#35)<br>
[3-6. 什么时候会使用 Core Graphics,有什么注意事项么?](#36)<br>
[3-7. NSNotification 和 KVO 的使用场景?](#37)<br>
[3-8. 使用 Block 时需要注意哪些问题?优点?具体实现?](#38)<br>
[3-9. performSelector: withObject: afterDelay: 内部大概是怎么实现的,有什么注意事项么?](#39)<br>
[3-10. 如何播放 GIF 图片,有什么优化方案么?](#310)<br>
[3-11. 使用 NSUserDefaults 时,如何处理布尔的默认值?(比如返回 NO,不知道是真的 NO 还是没有设置过),及简介](#311)<br>
[3-12. 有哪几种方式可以对图片进行缩放,使用 CoreGraphics 缩放时有什么注意事项?](#312)<br>
[3-13. 哪些途径可以让 ViewController 瘦下来?](#313)<br>
[3-14. 有哪些常见的 Crash 场景?](#314)<br>

##综合类问题
[4-1. 设计一个可以无限滚动并且支持自动滚动的 SliderShow](#41)<br>
[4-2. 设计一个进度条](#42)<br>
[4-3. 设计一套大文件（如上百M的视频）下载方案](#43)<br>
[4-4. 如果让你来实现 dispatch_once,你会怎么做？](#44)<br>
[4-5. 设计一个类似 iOS 主屏可以下拉出现 Spotlight 的系统.(对 UIScrollView 的理解程度)](#45)

#Answer
###吾三跪
<hr>

<p id="5" style="color: blue"><b>1-5. 最常用的版本控制工具是什么,能大概讲讲原理么?</b></p>
	
	版本控制工具: Git
	从根本上来讲 Git 是一套内容寻址 (content-addressable) 文件系统,在此之上提供了一个 VCS 用户界面
详细见 <a href="https://git-scm.com/book/zh/v1/Git-%E5%86%85%E9%83%A8%E5%8E%9F%E7%90%86" style="color: #B2AB23">Git 原理</a>	

<p id="7" style="color: blue"><b>1-7. 你一般是怎么用 Instruments 的?</b></p>
	
	Time Profiler 查看代码&耗时详情
	Leaks 检测内存泄漏,不得不吐槽 QQ-SDK, 之前的项目上架前,查出 37 个 New Leaks, 定位发现, QQSDK 版本更新了, 并且没有通知我...
关于 Leaks 的使用<a href="http://www.jianshu.com/p/c0aa12d91f05" style="color: #B2AB23">见这篇文章</a>

<p id = "10" style="color: blue"><b>1-10 如何实现单例,单例会有什么弊端?</b></p>

	·单例相当于全局变量,因此存在强耦合,不利于扩展和应对变化
	·单例违背单一设计原则

###知识性问题
<hr>
<p id="21" style="color: blue"><b>2-1 什么是响应链,它是怎么工作的?</b></p>
	
	事件的传递顺序是这样的:
	产生触摸事件 -> UIApplication 事件队列 -> [UIApplication hitTest: withEvent:] -> 返回更合适的 view -> [子控件 hitTest: withEvent:] -> 返回更合适的 view
<p id="23"></p>
<p id="24" style="color: blue"><b>2-4 如何把一个包含自定义对象的数组序列化到磁盘？</b></p>
	
	自定义对象需要实现 NSCoding 协议,然后可以调用 NSKeyedArchiver +(BOOL)archiveRootObject:(id)rootObject toFile:(NSString *)path 
	方法将它序列化到磁盘

<p id="25" style="color: blue"><b>2-5. Apple Pay 是什么？它的大概工作流程是怎样的?</b></p>

	购买流程:
		1.程序向服务器发送请求,获得一份产品列表.
		2.服务器返回包含产品标识符的列表.
		3.程序向 App Store 发送请求,得到产品的信息.
		4.App Store 返回产品信息.
		5.程序把返回的产品信息显示给用户(App 的 store 界面)
		6.用户选择某个产品.
		7.程序向 App Store 发送支付请求.
		8.App Store 处理支付请求并返回交易完成信息.
		9.程序从信息中获得数据,并发送至服务器.
		10.服务器纪录数据,并进行审(我们的)查.
		11.服务器将数据发给 App Store 来验证该交易的有效性.
		12.App Store 对收到的数据进行解析,返回该数据和说明其是否有效的标识.
		13.服务器读取返回的数据,确定用户购买的内容.
		14.服务器将购买的内容传递给程序.

	注意事项:
		1.掉单的相关处理,因为网速-延迟等原因,造成用户花了钱,没有得到商品
  			1).将交易凭证存在本地,在 rootViewController 监听 SKPaymentTransactionObserver  
  			[[SKPaymentQueue defaultQueue]addTransactionObserver:self];

  			2).判断
  			if (transaction.transactionState == SKPaymentTransactionStatePurchased) {
       	 		NSLog(@"-----completeTransaction--------");
        		// Your application should implement these two methods.
        		NSString *product = transaction.payment.productIdentifier;
       			NSString * receipt = nil;
       			NSURLRequest*appstoreRequest = [NSURLRequest requestWithURL:[[NSBundle mainBundle]appStoreReceiptURL]];
       			NSError *error = nil;
       			NSData * receiptData = [NSURLConnection sendSynchronousRequest:appstoreRequest returningResponse:nil error:&error];
       			receipt = [receiptData base64EncodedStringWithOptions:NSDataBase64EncodingEndLineWithLineFeed];
       		    // your code,(我是将交易凭证和订单号一起发给服务器)
       		}
       		别忘了移除监听 [[SKPaymentQueue defaultQueue]removeTransactionObserver:self];


<p id="26" style="color: blue"><b>2-6 iOS 的沙盒目录结构是怎样的? App Bundle 里面都有什么？</b><br></p>
	
	(1) Bundle Path [APP 包]
		不属于沙盒目录,存放的是编译后的源文件,包括资源文件和可执行文件
		NSString *bundlePath = [[NSBundle mainBundle]bundlePath];

	(2) Home [App 沙盒根目录]
		NSString *homeStr = NSHomeDirectory();
	
	(3) Home -> Documents [文件目录]
		最常用的目录,iTunes 同步该 App 时会同步此目录中的内容,适合存储重要数据.使用场景比如：存储 SQLite 生成的数据库文件.
		NSString *documentStr = [NSSearchPathForDirectoriesInDomains(NSDocumentDirectory, NSUserDomainMask, YES)lastObject];

	(4) Home -> Library [库目录]
		NSString *libraryStr = [NSSearchPathForDirectoriesInDomains(NSLibraryDirectory, NSUserDomainMask, YES)lastObject];

	(5) Home -> Library -> Caches [缓存目录]
		iTunes 同步该 App 时不会同步此目录的内容,适合存储体积大,不需要备份的非重要数据<br>
		NSString *cacheStr = [NSSearchPathForDirectoriesInDomains(NSCachesDirectory,NSUserDomainMask, YES)lastObject];

	(6) Home -> Library -> Preferences [偏好设置目录]
		iTunes 同步该 App 时会同步此目录中的内容,通常保存 App 的偏好设置信息.使用场景比如:记录已登录的 App 用户的信息,非敏感信息,比如已登录状态.
		PS:Preferences 没有相对应的取目录方法,因为该目录主要存储用户「偏好设置」信息,可以直接通过键值对进行读写访问,因此也不需要获取目录.
	
	(7) Home -> Temp [临时目录]
		iTunes 同步该 App 时不会同步此目录中的内容,系统可能在 App 没运行的某个时机就删除该目录的文件,适合存储临时性的数据,用完就删除.
		使用场景比如：读取网络图片时,一般会先把图片作为临时文件下载存储到此目录,然后再拷贝临时文件到 Caches「缓存目录」下,拷贝完成后再删除此临时文件.

		这样做的目的是保证数据的原子性,我们常用的保存数据到文件的方法:writeToFile:,常常设置 atomically 参数值为 YES 也是这样的目的.
		NSString *tempStr = NSTemporaryDirectory();

<p id="27" style="color: blue"><b>2-7 iOS 的签名机制大概是怎样的？</b></p>
	
	签名机制：
	1.先将应用内容通过炸药算法,得到摘要
	2.再用私钥对摘要进行加密得到密文
	3.将原文本、密文和私钥对应的公钥一并发布

	验证流程：
	1.查看公钥是否是私钥方的
	2.然后用公钥对密文进行解密得到摘要
	3.将 App 用同样的摘要算法得到摘要,两个摘要进行对比,如果相等那么一切正常.

	以上过程只要有一步出问题就视为无效

<p id="28" style="color: blue"><b>2-8 iOS 7的多任务添加了哪两个新的 API? 各自的使用场景是什么？</b></p>
	
	后台获取（Background Fetch):
	后台获取使用场景是用户打开应用之前就使 app 有机会执行代码来获取数据,刷新 UI.这样在用户打开应用的时候,最新的内容将已然呈现
	在用户眼前,而省去了所有的加载过程

	推送唤醒（Remote Notifications):
	使用场景是使设备在接收到远端推送后让系统唤醒设备和我们的后台应用,并先执行一段代码来准备数据和 UI,然后再提示用户有推送.
	这时用户如果解锁设备进入应用后将不会再有任何加载过程,新的内容将直接得到呈现

<p id="29" style="color: blue"><b>2-9 Objective-C 的 class 是如何实现的？Selector 是如何被转化为 C 语言的函数调用的？</b></p>
	
	[receive message] => objc_msgSend(receiver,selector);

<p id="210" style="color: blue"><b>2-10 UIScrollView 大概是如何实现的,它是如何捕捉、响应手势的？</b></p>
	
	1.实现原理:
	1). UIScrollView 在滚动的过程中,其实是在修改原点坐标.当手指触摸后,scrollView 会暂时拦截触摸事件,使用一个计时器.
	
	2). 假如在计时器到点后没有发生手指移动事件,那么 scrollView 发送 tracking event 到被点击的 subview.
	
	3). 假如在计时器到点前发生了移动事件,那么 scrollView 取消 tracking 自己发生滚动.
	
	2.事件
	1). UIScrollView 应该是重载了 hitTest 方法,并总会返回 itSelf.所以所有的 touch 事件都会进入到它自己里面去了.
	内部的 touch 事件检测到这个事件是不是和自己相关的,或者处理或者传递给内部的 view
	
	2). 为了检测 touch 是处理还是传递,它就把这个事件传递给内部 view
	
	3). 如果 150ms 内 touch 产生移动,开始 scrolling,不会传递给内部的 view（假如,当你 touch 一个 tableView,
	之间 scrolling,你 touch 的那行永远不会 highlight）
	
	4). 如果 150ms 内 touch 未产生移动并且 UIScrollView 开始传递内部的 view 事件,但是移动足够远点话,且 
	canCancelContentTouches = YES, UIScrollView 会调用 touchesCancelled 方法,cancel 掉内部 view 的事件响应,并开始 scrolling.
	（例如,当你 touch 一个 tableView,停止了一会,然后开始 scrolling.那一行就首先 highlight,但是随后就不在高亮了）

<p id="211" style="color: blue"><b> 2-11 Objective-C 如何对已有的方法,添加自己的功能代码以实现类似记录日志这样的功能？</b></p>
	
	这题目主要考察的是 runtime 如何交换方法
	+ (NSString *)myLog	{

	}

	+ (void)load {
		//获取 description 方法地址
		Method description = class_getClassMethod(self, @selector(description));

		//获取 myLog 方法地址
		Method myLog = class_getClassMethod (self, @selector(myLog));

		//交换方法地址,相当于交换实现方式
		method_exchangeImplementations(description, myLog);
	}

<p id="212" style="color: blue"><b>2-12 +load 和 +initialize 的区别是什么？</b></p>
	
	+ (void)load;
	1. 当类对象被引入项目时, runtime 会向每一个类对象发送 load 消息
	load 方法会在每一个类甚至分类被引入时仅调用一次,调用的顺序:父类优先于子类,子类优先于分类
	2. load 方法不会被类自动继承

	+ (void)initialize;
	也是在第一次使用这个类的时候会调用这个方法

<p id="213" style="color: blue"><b>2-13. 如何让 Category 支持属性?</b></p>
	
	使用 Runtime 可以实现

<p id="214" style="color: blue"><b>2-14 NSOperation 相比于 GCD 有哪些优势？</b></p>
	
	1.可以取消操作
	2.可以更容易的添加任务的依赖关系
	3.可以 KVO 属性
	4.可以添加优先级
	5.可以复用

<p id="215" style="color: blue"><b>2-15 strong / weak / unsafe_unretained 的区别?</b></p>
	
	· weak 只能修饰 OC 对象,使用 weak 不会使计数器加 1,对象销毁时修饰的对象会指向 nil
	· strong 等价与 retain,能使计数器加 1,且不能用来修饰数据类型
	· unsafe_unretained 等价与 assign,可以用来修饰数据类型和 OC 对象,但是不会使计数器加 1,
	且对象销毁时也不会将对象指向 nil,容易造成野指针错误

<p id="216" style="color: blue"><b>2-16 如何为 Class 定义一个对外只读对内可读写的属性?</b>
</p>
	
	在头文件中将属性定义为 readonly,在 .m 文件中将属性重新定义为 readwrite

<p id="217" style="color: blue"><b>2-17. Objective-C 中,meta-class 指的是什么?</b></p>
<img src="/Resource/meta-class.png">

	元类(metaclass)也是一个对象,那么元类的 isa 指针又指向哪里呢?
	为了设计上的完整，所有的元类的 isa 指针都会指向一个根元类(root metaclass).
	根元类(root metaclass)本身的 isa 指针指向自己,这样就行成了一个闭环.
	上面提到,一个对象能够接收的消息列表是保存在它所对应的类中的.
	在实际编程中,我们几乎不会遇到向元类发消息的情况,那它的 isa 指针在实际上很少用到.
	不过这么设计保证了面向对象的干净,即所有事物都是对象,都有 isa 指针

<p id="218" style="color: blue"><b>2-18 UIView 和 CALayer 之间的关系?</b></p>

	1.每个 UIView 内部都有一个 CALayer 在背后提供内容的绘制和显示,并且 UIView 的尺寸样式都由内部的 Layer 所提供.
	两者都有树状层级结构, layer 内部有 SubLayers, View 内部有 SubViews.但是 Layer 比 View 多了个 AnchorPoint
	
	2.在 View 显示的时候, UIView 做为 Layer 的 CALayerDelegate, View 的显示内容由内部的 CALayer 的 display
	
	3.CALayer 是默认修改属性支持隐式动画的,在给 UIView 的 Layer 做动画的时候, View 作为 Layer 的代理,
	Layer 通过 actionForLayer: forKey: 向 View 请求相应的 action(动画行为)
	
	4.layer 内部维护着三分 layer tree,分别是 presentLayer Tree(动画树),modeLayer Tree(模型树), Render Tree (渲染树).
	在做 iOS动画的时候,我们修改动画的属性,在动画的其实是 Layer 的 presentLayer 的属性值,而最终展示在界面上的其实是提供 View 的 modelLayer
	
	5.两者最明显的区别是 View 可以接受并处理事件,而 Layer 不可以

<p id="220" style="color: blue"><b>2-20. @property (copy)NSMutableArray *array; 这个写法会出什么问题?
</b></p>

	1.添加/删除/修改数组内的元素的时候,程序会因为找不到对应的方法而奔溃,因为 copy 就是复制不可变的 NSArray 对象
	2.使用了 atomic 属性会严重影响性能.
   	如果属性具备 nonatomic 特质,则不使用同步锁.
   	如果属性不具备 nonatomic 特质,那它就是”原子的(atomic)”

<p id="221" style="color: blue"><b>2-21. const 和 define 的区别?</b></p>

	1. const 在编译阶段使用, define 在预编译阶段使用
	2. const 有数据类型,作安全检查; define 无类型,不作安全检查
	3. const 可以调试; define 不能调试
	4. const 占用一份内存; define 有若干个拷贝

<p id="222" style="color: blue"><b>2-22. 讲述一下 runtime 的概念, message send 如果寻找不到相应的对象,会如何进行后续处理?</b></p>

<a href="https://github.com/slodier/RuntimeNote" target="_blank" style="color: #B2AB23">详细看这篇文章</a>

###经验类问题
<hr>
<p id="31" style="color: blue"><b>3-1 为什么 UIScrollView 的滚动会导致 NSTimer 失效?</b>
</p>

	因为 UIScrollView 滚动的时候跟主线程不是同一个 runloop mode,一个 runloop mode 就是 input sources、timer 和 observers 的集合.
	每次执行 runloop,都需要指定一个 mode. 
	UIScrollView 滚动时候由于不同的 mode 所以也导致它只能保证它所在的 runloop 的 timer 有效,而主线程无效.
	解决方法:
	[NSRunLoop currentRunLoop]addTimer:_openTimer forMode:UITrackingRunLoopMode];

<p id="33" style="color: blue"><b>3-3 你会如何存储用户的一些敏感信息,如登录的 token.</b>
</p>
<a href="https://github.com/slodier/CCKeychain" target="_blank" style="color: #B2AB23">放个链接</a>

<p id="39" style="color: blue"><b>3-9 performSelector: withObject: afterDelay: 内部大概是怎么实现的,有什么注意事项么?</b></p>

	创建一个定时器,时间结束后系统会使用 Runtime 通过方法名称(Selector 本质就是方法名称)去方法列表中找到对应的方法调用并实现
注意事项:
	
	1.调用 performSelector: withObject: afterDelay: 方法时,先判断希望调用的方法是否存在 respondsToSelector:
	
	2.这个方法是异步方法,必须在主线程调用,在子线程调用永远不会调用该方法


<p id="310" style="color: blue"><b>3-10 如何播放 GIF 图片,有什么优化方案么？</b>
</p>
<a href="http://www.cnblogs.com/asamu/p/6046729.html" target="_blank" style="color: #B2AB23">优化方案</a>

<p id="311" style="color: blue"><b>3-11. 使用 NSUserDefaults 时,如何处理布尔的默认值?(比如返回 NO,不知道是真的 NO 还是没有设置过),及简介</b></p>

	在 NSUserDefaults 中设置 BOOL 类型的值总会有一个非常麻烦的问题. 如果我们要在 NSUserDefaults 中存储一个 BOOL 类型的值,
	当我们使用 boolForKey: 取出它的值时, 它的默认值总是 (nil)NO.
	因为在你没有为一个 key 单独设置值时, 它的默认值总是 nil. 所以在我们使用 NSUserDefaults 设置一个 BOOL 值时, 总会把这个 
	BOOL 值的 语义设置为相反的.
	但是当我们需要把 BOOL 值的默认值设置为 YES 时, 其实也是有办法的.

	if ([[NSUserDefaults standUserDefaults] objectForKey:xxx] == nil) {  
   	 [[NSUserDefaults standUserDefaults] setBool:YES forKey:xxx];
	}

##未完待续...