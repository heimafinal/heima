
<!DOCTYPE html>
<html lang="zh-CN">
    <!-- title -->




<!-- keywords -->




<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no" >
    <meta name="author" content="Zhangguanzhang">
    <meta name="renderer" content="webkit">
    <meta name="copyright" content="Zhangguanzhang">
    
    <meta name="keywords" content="hexo,hexo-theme,hexo-blog">
    
    <meta name="description" content="记录生活点滴">
    <meta name="description" content="记录生活点滴">
<meta property="og:type" content="website">
<meta property="og:title" content="Zhangguanzhang">
<meta property="og:url" content="http://zhangguanzhang.github.io/">
<meta property="og:site_name" content="Zhangguanzhang">
<meta property="og:description" content="记录生活点滴">
<meta property="og:locale" content="zh_CN">
<meta property="article:author" content="Zhangguanzhang">
<meta name="twitter:card" content="summary">
    <meta http-equiv="Cache-control" content="no-cache">
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"/>
    
    <title>zhangguanzhang&#39;s Blog</title>
    <style type="text/css">
    @font-face {
        font-family: 'Oswald-Regular';
        src: url("/font/Oswald-Regular.ttf");
    }

    body {
        margin: 0;
    }

    header,
    footer,
    .back-top,
    .sidebar,
    .container,
    .site-intro-meta,
    .toc-wrapper {
        display: none;
    }

    .site-intro {
        position: relative;
        z-index: 3;
        width: 100%;
        /* height: 50vh; */
        overflow: hidden;
    }

    .site-intro-placeholder {
        position: absolute;
        z-index: -2;
        top: 0;
        left: 0;
        width: calc(100% + 300px);
        height: 100%;
        background: repeating-linear-gradient(-45deg, #444 0, #444 80px, #333 80px, #333 160px);
        background-position: center center;
        transform: translate3d(-226px, 0, 0);
        animation: gradient-move 2.5s ease-out 0s infinite;
    }

    @keyframes gradient-move {
        0% {
            transform: translate3d(-226px, 0, 0);
        }
        100% {
            transform: translate3d(0, 0, 0);
        }
    }

</style>

    <link rel="preload" href= "/css/style.css?v=20180824" as="style" onload="this.onload=null;this.rel='stylesheet'" />
    <link rel="stylesheet" href= "/css/mobile.css?v=20180824" media="(max-width: 980px)">
    
    <!-- /*! loadCSS. [c]2017 Filament Group, Inc. MIT License */
/* This file is meant as a standalone workflow for
- testing support for link[rel=preload]
- enabling async CSS loading in browsers that do not support rel=preload
- applying rel preload css once loaded, whether supported or not.
*/ -->
<script>
(function( w ){
	"use strict";
	// rel=preload support test
	if( !w.loadCSS ){
		w.loadCSS = function(){};
	}
	// define on the loadCSS obj
	var rp = loadCSS.relpreload = {};
	// rel=preload feature support test
	// runs once and returns a function for compat purposes
	rp.support = (function(){
		var ret;
		try {
			ret = w.document.createElement( "link" ).relList.supports( "preload" );
		} catch (e) {
			ret = false;
		}
		return function(){
			return ret;
		};
	})();

	// if preload isn't supported, get an asynchronous load by using a non-matching media attribute
	// then change that media back to its intended value on load
	rp.bindMediaToggle = function( link ){
		// remember existing media attr for ultimate state, or default to 'all'
		var finalMedia = link.media || "all";

		function enableStylesheet(){
			link.media = finalMedia;
		}

		// bind load handlers to enable media
		if( link.addEventListener ){
			link.addEventListener( "load", enableStylesheet );
		} else if( link.attachEvent ){
			link.attachEvent( "onload", enableStylesheet );
		}

		// Set rel and non-applicable media type to start an async request
		// note: timeout allows this to happen async to let rendering continue in IE
		setTimeout(function(){
			link.rel = "stylesheet";
			link.media = "only x";
		});
		// also enable media after 3 seconds,
		// which will catch very old browsers (android 2.x, old firefox) that don't support onload on link
		setTimeout( enableStylesheet, 3000 );
	};

	// loop through link elements in DOM
	rp.poly = function(){
		// double check this to prevent external calls from running
		if( rp.support() ){
			return;
		}
		var links = w.document.getElementsByTagName( "link" );
		for( var i = 0; i < links.length; i++ ){
			var link = links[ i ];
			// qualify links to those with rel=preload and as=style attrs
			if( link.rel === "preload" && link.getAttribute( "as" ) === "style" && !link.getAttribute( "data-loadcss" ) ){
				// prevent rerunning on link
				link.setAttribute( "data-loadcss", true );
				// bind listeners to toggle media back
				rp.bindMediaToggle( link );
			}
		}
	};

	// if unsupported, run the polyfill
	if( !rp.support() ){
		// run once at least
		rp.poly();

		// rerun poly on an interval until onload
		var run = w.setInterval( rp.poly, 500 );
		if( w.addEventListener ){
			w.addEventListener( "load", function(){
				rp.poly();
				w.clearInterval( run );
			} );
		} else if( w.attachEvent ){
			w.attachEvent( "onload", function(){
				rp.poly();
				w.clearInterval( run );
			} );
		}
	}


	// commonjs
	if( typeof exports !== "undefined" ){
		exports.loadCSS = loadCSS;
	}
	else {
		w.loadCSS = loadCSS;
	}
}( typeof global !== "undefined" ? global : this ) );
</script>

    <link rel="icon" href= "/assets/favicon.ico" />
    <link rel="preload" href="https://cdn.jsdelivr.net/npm/webfontloader@1.6.28/webfontloader.min.js" as="script" />
    <link rel="preload" href="https://cdn.jsdelivr.net/npm/jquery@3.3.1/dist/jquery.min.js" as="script" />
    <link rel="preload" href="/scripts/main.js" as="script" />
    <link rel="preload" as="font" href="/font/Oswald-Regular.ttf" crossorigin>
    <link rel="preload" as="font" href="https://at.alicdn.com/t/font_327081_1dta1rlogw17zaor.woff" crossorigin>
    
    <!-- fancybox -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/fancybox/3.2.5/jquery.fancybox.min.js" defer></script>
    <!-- 百度统计  -->
    
    <!-- 谷歌统计  -->
    
<meta name="generator" content="Hexo 5.3.0"><link rel="alternate" href="/atom.xml" title="Zhangguanzhang" type="application/atom+xml">
</head>

    
        <body class="home-body">
    
    
<header class="header index-header">

    <div class="read-progress"></div>
    <div class="header-sidebar-menu">&#xe775;</div>
    <!-- post页的toggle banner  -->
    
    <a class="home-link" href=/>zhangguanzhang's Blog</a>
</header>
    <div class="wrapper">
        <div class="site-intro" style="







height:50vh;
">
    
    <!-- 主页  -->
    
    
    <!-- 文章页  -->
            
    <div class="site-intro-placeholder"></div>
    <div class="site-intro-img" style="background-image: url(/intro/index-bg.jpg)"></div>
    <div class="site-intro-meta">
        <!-- 标题  -->
        <h1 class="intro-title">
            <!-- 主页  -->
            
            zhangguanzhang's Blog
            <!-- 文章页  -->
            
        </h1>
        <!-- 副标题 -->
        <p class="intro-subtitle">
            <!-- 主页副标题  -->
            
            
                站在巨人的肩膀上
            
            <!-- 文章页  -->
            
        </p>
        <!-- 文章页meta -->
        
    </div>
</div>
        <script>
 
  // get user agent
  var browser = {
    versions: function () {
      var u = window.navigator.userAgent;
      return {
        userAgent: u,
        trident: u.indexOf('Trident') > -1, //IE内核
        presto: u.indexOf('Presto') > -1, //opera内核
        webKit: u.indexOf('AppleWebKit') > -1, //苹果、谷歌内核
        gecko: u.indexOf('Gecko') > -1 && u.indexOf('KHTML') == -1, //火狐内核
        mobile: !!u.match(/AppleWebKit.*Mobile.*/), //是否为移动终端
        ios: !!u.match(/\(i[^;]+;( U;)? CPU.+Mac OS X/), //ios终端
        android: u.indexOf('Android') > -1 || u.indexOf('Linux') > -1, //android终端或者uc浏览器
        iPhone: u.indexOf('iPhone') > -1 || u.indexOf('Mac') > -1, //是否为iPhone或者安卓QQ浏览器
        iPad: u.indexOf('iPad') > -1, //是否为iPad
        webApp: u.indexOf('Safari') == -1, //是否为web应用程序，没有头部与底部
        weixin: u.indexOf('MicroMessenger') == -1, //是否为微信浏览器
        uc: u.indexOf('UCBrowser') > -1 //是否为android下的UC浏览器
      };
    }()
  }
  console.log("userAgent:" + browser.versions.userAgent);

  // callback
  function fontLoaded() {
    console.log('font loaded');
    if (document.getElementsByClassName('site-intro-meta')) {
      document.getElementsByClassName('intro-title')[0].classList.add('intro-fade-in');
      document.getElementsByClassName('intro-subtitle')[0].classList.add('intro-fade-in');
      var postIntros = document.getElementsByClassName('post-intros')[0]
      if (postIntros) {
        postIntros.classList.add('post-fade-in');
      }
    }
  }

  // UC不支持跨域，所以直接显示
  function asyncCb(){
    if (browser.versions.uc) {
      console.log("UCBrowser");
      fontLoaded();
    } else {
      WebFont.load({
        custom: {
          families: ['Oswald-Regular']
        },
        loading: function () {  //所有字体开始加载
          // console.log('loading');
        },
        active: function () {  //所有字体已渲染
          fontLoaded();
        },
        inactive: function () { //字体预加载失败，无效字体或浏览器不支持加载
          console.log('inactive: timeout');
          fontLoaded();
        },
        timeout: 5000 // Set the timeout to two seconds
      });
    }
  }

  function asyncErr(){
    console.warn('script load from CDN failed, will load local script')
  }

  // load webfont-loader async, and add callback function
  function async(u, cb, err) {
    var d = document, t = 'script',
      o = d.createElement(t),
      s = d.getElementsByTagName(t)[0];
    o.src = u;
    if (cb) { o.addEventListener('load', function (e) { cb(null, e); }, false); }
    if (err) { o.addEventListener('error', function (e) { err(null, e); }, false); }
    s.parentNode.insertBefore(o, s);
  }

  var asyncLoadWithFallBack = function(arr, success, reject) {
      var currReject = function(){
        reject()
        arr.shift()
        if(arr.length)
          async(arr[0], success, currReject)
        }

      async(arr[0], success, currReject)
  }

  asyncLoadWithFallBack([
    "https://cdn.jsdelivr.net/npm/webfontloader@1.6.28/webfontloader.min.js", 
    "https://cdn.bootcss.com/webfont/1.6.28/webfontloader.js",
    "/lib/webfontloader.min.js"
  ], asyncCb, asyncErr)
</script>        
        <img class="loading" src="/assets/loading.svg" style="display: block; margin: 6rem auto 0 auto; width: 6rem; height: 6rem;" />
        <div class="container container-unloaded">
            <main class="main index-page">
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2021/04/30/kubernetes-sec-agent-node-network-error/" >
            
                <span>一次单节点单个pod网络问题排查过程</span>
        </a>
        <div class="abstract-content">
            about现场反馈客户环境上业务不正常，根据调用链去看某个业务A日志，发现无法请求另一个业务B，把业务 A 的探针取消了，加上
12tty: truecommand: [&quot;bash&quot;]
起来后进去 curl 了下 B 对应的 svcIP 接口是能通的。然后手动起业务进程，再开个窗口 exec 进去 curl 发现就不通了，k8s node数量是只有一个，并且只有这一个 pod 有问题。后面排查到是用户的安全软件导致的。软件名是
1234567$ ps aux | grep agentroot       6349  0.3  0.1 21046316 116820 ?...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2021/04/30</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "k8s">k8s</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2021/04/08/kubelet-runc-disable-kmem/" >
            
                <span>kubelet 和 runc 编译关闭 kmem</span>
        </a>
        <div class="abstract-content">
            前提详情在 3.x 的内核上，cgroup 的 kmem account 特性有内存泄露问题。kubelet 和 runc 都需要修复。
网上有言论说升级 Linux 内核至 kernel-3.10.0-1075.el7 及以上就可以修复这个问题，详细可见 slab leak causing a crash when using kmem control group。但是我测试了下面的都不行：

CentOS7.4
CentOS7.6
CentOS7.7的 3.10.0-1062.el7.x86_64 
CentOS Linux release 7.8.2003 (Core) - 3.1...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2021/04/08</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "k8s">k8s</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2021/03/23/iptables-docker-no-chain/" >
            
                <span>iptables --wait -t nat -A DOCKER...: iptables NO chain/target/match by that name</span>
        </a>
        <div class="abstract-content">
            由来我们内部有套部署的工具， 我们部署的流程是先在部署机器（部署机器可能也是node1 ）上用脚本安装好 docker，然后进容器里去起我们部署平台，有个很久的 bug 就是，部署机器上端口映射起容器会有如下报错
1iptables --wait -t nat -A DOCKER -p tcp -d 0&#x2F;8 --dport 8089 -j DNAT --to-destination 172.25.0.2:80 ! -i docker0: iptables NO chain&#x2F;target&#x2F;match by that name
排查也很简单，缺少链，添加上即可:...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2021/03/23</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "k8s">k8s</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2021/03/22/jsonpatch-doc-is-missing-path/" >
            
                <span>Internal error occurred: jsonpatch add operation does not apply: doc is missing path: xxx</span>
        </a>
        <div class="abstract-content">
            由来今天在折腾 admission webhook 注入一些属性的时候遇到了 Error from server (InternalError): error when creating &quot;xxx.yml&quot;: Internal error occurred: jsonpatch add operation does not apply: doc is missing path: &quot;/spec/template/spec/dnsConfig/options&quot;。折腾半天才发现在代码里使用 jsonPatch 的话不能直接绕过结构体实例去 patch。 ...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2021/03/22</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "k8s">k8s</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2021/03/12/build-arm64-docker-compose-action/" >
            
                <span>使用github action 配合 docker buildx 编译 arm64 docker-compose</span>
        </a>
        <div class="abstract-content">
            说明git 上搜索了很多 docker-compose 的 arm64 的编译基本都是使用 qemu-user-static 之类的设置下后编译的，也看到过用特权容器启动 qemu-user-static 或者 binfmt 之类的，但是我自己机器上试了无效，貌似是因为我操作系统是低版本内核的 centos ，github 上搜了下，其他很多人的编译感觉太啰嗦了。就在 action 上整了下，测试是可用的，而且非常简单。
docker-practice/actions-setup-docker@master 将会在在 action 的 runner 里安装 docker，创建 build...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2021/03/12</span>
            </div>
            <!-- tags  -->
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2021/02/02/node-shutdown-dns-unavailable/" >
            
                <span>集群节点关机导致dns在eviction pod之前几率不可用</span>
        </a>
        <div class="abstract-content">
            由来这几天我们内部在做新项目的容灾测试，业务都是在 K8S 上的。容灾里就是随便选节点 shutdown -h now。关机后同事便发现了（页面有错误，最终问题是）集群内 DNS 解析会有几率无法解析（导致的）。
根据 SVC 的流程，node 关机后，由于 kubelet 没有 update 自己。node 和 pod 在 apiserver get 的时候显示还是正常的。在 kube-controller-manager 的 --node-monitor-grace-period 时间后再过 --pod-eviction-timeout 时间开始 eviction pod，大概流程是...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2021/02/02</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "coredns">coredns</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2020/12/04/docker1803-hang-container-restore/" >
            
                <span>docker18.03 hang at &#39;restoring container&#39;</span>
        </a>
        <div class="abstract-content">
            由来起初是 k8s 有几个 node not ready，上去看了下 kubelet 日志刷 container runtime down，重启了下 docker 后还是没用，docker ps 命令都卡住。
环境信息1234567891011121314151617181920212223242526272829303132333435363738394041424344454647484950515253$ cat /etc/redhat-release Linux xxx-disk0 3.10.0-1127.13.1.el7.x86_64 #1 SMP Tue Jun 23 15:...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2020/12/04</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "hang">hang</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2020/11/23/ansible-hang-in-docker/" >
            
                <span>ansible hang in docker container</span>
        </a>
        <div class="abstract-content">
            由来这几天同事发现在 docker 容器里运行 ansible 命令很卡，发来了个命令叫我试试 ansible localhost -m setup -a &#39;filter=ansible_default_ipv4&#39; 2&gt;/dev/null |grep &#39;\&quot;address\&quot;&#39; |awk -F&#39;\&quot;&#39; &#39;&#123;print $4&#125;&#39;
环境信息12345678910111213141516171819202122232425262728293031323334353637383...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2020/11/23</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "docker">docker</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2020/11/20/disable-swap/" >
            
                <span>永久关闭swap的正确姿势</span>
        </a>
        <div class="abstract-content">
            今天遇到了 kylin 系统上无法关闭 swap 的情况。记录下和方便别人搜到这个知识点。
环境信息1234$ at /etc/issueKylin 4.0.2 \n \l$ uname -aLinux H-192-168-63-132 4.15.0- 58-generic #64kord1k1&#x27;SMP Thu Aug 1S15:51:97 csT 2919 aarch64 ......
尝试的步骤fstab 里没有 swap 的挂载，
1swapoff -a &amp;&amp; sysctl -w vm.swappiness=0
重启后，内核参数是关闭的，但是实际没有关闭
...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2020/11/20</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "swap">swap</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2020/11/06/kylin-arm-clone-vxlan-error/" >
            
                <span>银河麒麟arm64系统克隆机器上k8s vxlan跨节点不通的一次排查</span>
        </a>
        <div class="abstract-content">
            由来和前一篇文章不一样，从来没遇到过这样的问题，这里记录下。实施在客户那边部署业务后，业务在浏览器上无法访问，我远程上去查看日志发现 pod 内部无法 DNS 无法解析，nginx 连不上 upsteam 报错而启动失败，实际上也是跨节点不通。实际排查过程也有往错误的方向浪费了一些时间和尝试，就不写进来了，以正确的角度写下排查过程。
环境信息OS 是 arm64 的银河麒麟系统：
123456789$ cat /etc/os-releaseNAME="Kylin Linux Advanced Server"VERSION="V10 (Tercel)"ID="kylin"VERSION_I...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2020/11/06</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "Kylin">Kylin</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2020/10/30/uos20-nftables/" >
            
                <span>统信USO 20 hostPort 无法访问</span>
        </a>
        <div class="abstract-content">
            由来这些天陆续发现很多客户是统信的系统，部署我们业务后无法访问
环境信息我自己环境和客户的环境都遇到了无法访问，我自己测试的机器信息是:
1234567891011$ cat /etc/os-releasePRETTY_NAME=&quot;Uniontech OS Server 20 Enterprise&quot;NAME=&quot;Uniontech OS Server 20 Enterprise&quot;VERSION_ID=&quot;20&quot;VERSION=&quot;20&quot;ID=UOSHOME_URL=&quot;https://www.chinauo...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2020/10/30</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "uos">uos</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2020/10/20/kylin-v10-k8s-overlay-error/" >
            
                <span>银河麒麟arm64系统上k8s集群跨节点不通的一次排查</span>
        </a>
        <div class="abstract-content">
            由来同事在客户那边部署的集群问题频繁，先给他解决了个问题后又反映说业务 POD 由于 DNS 无法解析而启动失败，排查完发现这样的情况从没遇到过，挺有意思的，这里记录下。实际排查过程也有往错误的方向浪费了一些时间和尝试，就不写进来了，以正确的角度写下排查过程。
环境信息集群信息:
12345678910111213141516171819202122232425$ kubectl version -o json&#123;  &quot;clientVersion&quot;: &#123;    &quot;major&quot;: &quot;1&quot;,    &quot;mi...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2020/10/20</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "Kylin">Kylin</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2020/09/18/ocp-4.5-install/" >
            
                <span>openshift 4.5.9 离线安装</span>
        </a>
        <div class="abstract-content">
            本文是全部离线安装，也就是 UPI (User Provisioned Infrastructure) 模式安装，假设机器只能配置静态ip不能有网络配置权限和配置 dhcp 和 pxe。机器可以是物理机和虚拟机。
前言介绍ocp介绍openshift 分为社区版本 okd 和企业版本 ocp(openshift container platform)，okd 的更新很慢，ocp 个人也是可以安装的，不购买 license 则不会享受 redhat 的官方支持。
openshift 不像其他的 dashboard 诸如 rancher，k3s 之类的，它自己实现了 cs 的三个组件，也给 ...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2020/09/18</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "openshift">openshift</a>
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "ocp">ocp</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2020/08/05/wireguard-for-personal/" >
            
                <span>个人办公用 wireguard 组网笔记</span>
        </a>
        <div class="abstract-content">
            作为 IT 人员，经常需要连到办公网工作，并不是每个公司都有 vpn，自己搭建的话 openvpn 之类的配置麻烦啰嗦。这里写下 wireguard 的简单搭建。它比 IPSec 更快，更简单，更精简，更有用。它比 OpenVPN 更高效。WireGuard 设计为通用 VPN，适用于多种不同情况。它是跨平台的，可大规模部署。
通常如下图的部署: 一台 ECS 主机，得有公网 IP，下图就是 pc ----&gt; ECS &lt;------ 公司的 pc
12345678910111213141516            +----------+            |     ...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2020/08/05</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "wireguard">wireguard</a>
    
</div>
            
        </div>
    </article>
    
    
    
    
    
    
    <article class="index-post">
        <a class="abstract-title" href = "/2020/07/30/prometheus-rate-and-irate/" >
            
                <span>prometheus的rate与irate内部是如何计算的</span>
        </a>
        <div class="abstract-content">
            由来市面上的翻译误导人，压根不是啥平均增长率，看了下源码和实际算下来让大家好理解
rate主要代码是在 https://github.com/prometheus/prometheus/blob/master/promql/functions.go 的extrapolatedRate 和 funcRate，funcRate为
123func funcRate(vals []parser.Value, args parser.Expressions, enh *EvalNodeHelper) Vector &#123;  return extrapolatedRate(vals, args...
        </div>
        <div class="abstract-post-meta">
            <!-- date  -->
            <div class="abstract-date">
                <span class="abstract-calander iconfont-archer">&#xe676;</span><span class="abstract-time">2020/07/30</span>
            </div>
            <!-- tags  -->
            
            <div class= abstract-tags >
    
        <a class="post-tag" href="javascript:void(0);" data-tags = "Prometheus">Prometheus</a>
    
</div>
            
        </div>
    </article>
    
    <!-- paginator  -->
    
    <nav class="page-nav">
        <span class="page-number current">1</span><a class="page-number" href="/page/2/">2</a><a class="page-number" href="/page/3/">3</a><span class="space">&hellip;</span><a class="page-number" href="/page/7/">7</a><a class="extend next" rel="next" href="/page/2/">NEXT &gt;</a>
    </nav>
    
</main>
            <!-- profile -->
            
            <div class="profile">
    <img class="profile-avatar" alt="avatar" src= /avatar/dw.jpg >
    <div class="profile-name">Zhangguanzhang</div>
    
    <div class="profile-signature">
        on the way
    </div>
    
    
    <div class="profile-social">
        
    
        
            
                <a href="mailto:zhangguanzhang@qq.com" class="iconfont-archer email" title=email ></a>
            
        
    
        
            
                <a href="//github.com/zhangguanzhang" class="iconfont-archer github" target="_blank" title=github></a>
            
        
    
        
            
                <span class="iconfont-archer wechat" title=wechat>
                  
                  <img class="profile-qr" src="/assets/example_wc.png" />
                </span>
            
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
            
                <a href="/assets/zhifubao.png" class="iconfont-archer others" target="_blank" title=others></a>
            
        
    
        
            
                <a href="/atom.xml" class="iconfont-archer rss" target="_blank" title=rss></a>
            
        
    

    </div>
    
    
        <div class="friends">
            <div>FRIENDS</div>
            
                
                    <span>
                        <a href= //blog.cugxuan.cn target="_black">泫</a>
                    </span>
                
            
                
                    <span>
                        <a href= //linuxgeeks.github.io target="_black">传统老司机运维老村长</a>
                    </span>
                
            
                
                    <span>
                        <a href= //kuops.com target="_black">kuops</a>
                    </span>
                
            
                
                    <span>
                        <a href= //note.run-linux.com target="_black">Linus Lee</a>
                    </span>
                
            
                
                    <span>
                        <a href= //eryajf.net target="_black">二丫讲梵</a>
                    </span>
                
            
                
                    <span>
                        <a href= //www.k8stech.net target="_black">憨憨wolf7</a>
                    </span>
                
            
                
                    <span>
                        <a href= //sealyun.com/ target="_black">sealyun</a>
                    </span>
                
            
                
                    <span>
                        <a href= //blog.walkbc.com/ target="_black">golang后端dino</a>
                    </span>
                
            
                
                    <span>
                        <a href= https://blog.k8s.fit target="_black">Happiness</a>
                    </span>
                
            
                
                    <span>
                        <a href= //yousali.me target="_black">yousa</a>
                    </span>
                
            
                
                    <span>
                        <a href= //i4t.com target="_black">abcdocker</a>
                    </span>
                
            
        </div>
    
    
        <div class="about-me">
            <a href = "/about" >ABOUT ME</a>
        </div>
    
</div>
            
        </div>
        <footer class="footer footer-unloaded">
    <!-- social  -->
    
    <div class="social">
        
    
        
            
                <a href="mailto:zhangguanzhang@qq.com" class="iconfont-archer email" title=email ></a>
            
        
    
        
            
                <a href="//github.com/zhangguanzhang" class="iconfont-archer github" target="_blank" title=github></a>
            
        
    
        
            
                <span class="iconfont-archer wechat" title=wechat>
                  
                  <img class="profile-qr" src="/assets/example_wc.png" />
                </span>
            
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
    
        
            
                <a href="/assets/zhifubao.png" class="iconfont-archer others" target="_blank" title=others></a>
            
        
    
        
            
                <a href="/atom.xml" class="iconfont-archer rss" target="_blank" title=rss></a>
            
        
    

    </div>
    
    <!-- powered by Hexo  -->
    <div class="copyright">
        <span id="hexo-power">Powered by <a href="https://hexo.io/" target="_blank">Hexo</a></span><span class="iconfont-archer power">&#xe635;</span><span id="theme-info">theme <a href="https://github.com/fi3ework/hexo-theme-archer" target="_blank">Archer</a></span>
    </div>
    <!-- 不蒜子  -->
    
    <div class="busuanzi-container">
    
     
    <span id="busuanzi_container_site_pv">PV: <span id="busuanzi_value_site_pv"></span> :)</span>
    
    </div>
    
</footer>
    </div>
    <!-- toc -->
    
    <div class="back-top iconfont-archer">&#xe639;</div>
    <div class="sidebar sidebar-hide">
    <ul class="sidebar-tabs sidebar-tabs-active-0">
        <li class="sidebar-tab-archives"><span class="iconfont-archer">&#xe67d;</span><span class="tab-name">Archive</span></li>
        <li class="sidebar-tab-tags"><span class="iconfont-archer">&#xe61b;</span><span class="tab-name">Tag</span></li>
        <li class="sidebar-tab-categories"><span class="iconfont-archer">&#xe666;</span><span class="tab-name">Cate</span></li>
    </ul>
    <div class="sidebar-content sidebar-content-show-archive">
          <div class="sidebar-panel-archives">
    <!-- 在ejs中将archive按照时间排序 -->
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    <div class="total-and-search">
        <div class="total-archive">
        Total : 105
        </div>
        <!-- search  -->
        
    </div>
    
    <div class="post-archive">
    
    
    
    
    <div class="archive-year"> 2021 </div>
    <ul class="year-list">
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/30</span><a class="archive-post-title" href= "/2021/04/30/kubernetes-sec-agent-node-network-error/" >一次单节点单个pod网络问题排查过程</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/08</span><a class="archive-post-title" href= "/2021/04/08/kubelet-runc-disable-kmem/" >kubelet 和 runc 编译关闭 kmem</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/23</span><a class="archive-post-title" href= "/2021/03/23/iptables-docker-no-chain/" >iptables --wait -t nat -A DOCKER...: iptables NO chain/target/match by that name</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/22</span><a class="archive-post-title" href= "/2021/03/22/jsonpatch-doc-is-missing-path/" >Internal error occurred: jsonpatch add operation does not apply: doc is missing path: xxx</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/12</span><a class="archive-post-title" href= "/2021/03/12/build-arm64-docker-compose-action/" >使用github action 配合 docker buildx 编译 arm64 docker-compose</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">02/02</span><a class="archive-post-title" href= "/2021/02/02/node-shutdown-dns-unavailable/" >集群节点关机导致dns在eviction pod之前几率不可用</a>
        </li>
    
    
    
    
    
        </ul>
    
    <div class="archive-year"> 2020 </div>
    <ul class="year-list">
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">12/04</span><a class="archive-post-title" href= "/2020/12/04/docker1803-hang-container-restore/" >docker18.03 hang at 'restoring container'</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">11/23</span><a class="archive-post-title" href= "/2020/11/23/ansible-hang-in-docker/" >ansible hang in docker container</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">11/20</span><a class="archive-post-title" href= "/2020/11/20/disable-swap/" >永久关闭swap的正确姿势</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">11/06</span><a class="archive-post-title" href= "/2020/11/06/kylin-arm-clone-vxlan-error/" >银河麒麟arm64系统克隆机器上k8s vxlan跨节点不通的一次排查</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">10/30</span><a class="archive-post-title" href= "/2020/10/30/uos20-nftables/" >统信USO 20 hostPort 无法访问</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">10/20</span><a class="archive-post-title" href= "/2020/10/20/kylin-v10-k8s-overlay-error/" >银河麒麟arm64系统上k8s集群跨节点不通的一次排查</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">09/18</span><a class="archive-post-title" href= "/2020/09/18/ocp-4.5-install/" >openshift 4.5.9 离线安装</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">08/05</span><a class="archive-post-title" href= "/2020/08/05/wireguard-for-personal/" >个人办公用 wireguard 组网笔记</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">07/30</span><a class="archive-post-title" href= "/2020/07/30/prometheus-rate-and-irate/" >prometheus的rate与irate内部是如何计算的</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">07/23</span><a class="archive-post-title" href= "/2020/07/23/fs-error-fix-k8s-master/" >k8s master机器文件系统故障的一次恢复过程</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">06/23</span><a class="archive-post-title" href= "/2020/06/23/host-gw-in-aliyun/" >阿里云上使用flannel host-gw跨节点pod不通的解决</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">06/19</span><a class="archive-post-title" href= "/2020/06/19/go-prom-exporter/" >[未写完]使用go开发一个Prometheus的exporter</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">05/23</span><a class="archive-post-title" href= "/2020/05/23/k8s-vxlan-63-timeout/" >v1.17+ k8s集群下CNI使用VXLAN模式SVC有63秒延迟的触发原因定位</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">05/13</span><a class="archive-post-title" href= "/2020/05/13/x86-router-flash/" >proxmox x86软路由笔记</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">05/12</span><a class="archive-post-title" href= "/2020/05/12/N1-flash/" >斐讯N1刷机和旁路由的设置</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/27</span><a class="archive-post-title" href= "/2020/04/27/go-version-ifno/" >git工作流下golang项目的version信息该如何处理</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/26</span><a class="archive-post-title" href= "/2020/03/26/KubeXXXMismatch/" >一次deploy,rs,sts Mismatch 的处理</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/10</span><a class="archive-post-title" href= "/2020/03/10/go-mod-base-use/" >go mod的基础使用-科普</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/02</span><a class="archive-post-title" href= "/2020/03/02/centos6-hung-while-booting/" >centos6中毒重启后卡在启动页面</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/02</span><a class="archive-post-title" href= "/2020/03/02/binfmt-0000/" >记录一次request_module: runaway loop modeprobe binfmt-0000</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">02/27</span><a class="archive-post-title" href= "/2020/02/27/microsoft-graph-for-onedrive/" >使用microsoft-graph的api对接onedrive</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">01/08</span><a class="archive-post-title" href= "/2020/01/08/docker-panic-invalid-page-type/" >docker-18.06.3-ce启动panic: invalid page type: 0: 0的解决处理</a>
        </li>
    
    
    
    
    
        </ul>
    
    <div class="archive-year"> 2019 </div>
    <ul class="year-list">
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">12/05</span><a class="archive-post-title" href= "/2019/12/05/suse-fix-data-but-device-busy/" >opensuse的一次救援</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">12/03</span><a class="archive-post-title" href= "/2019/12/03/dos-to-gpt/" >从PTTYPE="dos"到TYPE="LVM2_member"的救援</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">11/24</span><a class="archive-post-title" href= "/2019/11/24/kubeadm-base-use/" >[长期更新]--应大多数人要求写下kubeadm的基础使用</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">10/24</span><a class="archive-post-title" href= "/2019/10/24/deployment-consul-in-k8s/" >consul仅当服务发现在k8s无状态部署使用</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">10/21</span><a class="archive-post-title" href= "/2019/10/21/k8s-v1.14-v1.15-fix-issue/" >手动修复v1.14-v1.15版本k8s的issue:76956</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">10/12</span><a class="archive-post-title" href= "/2019/10/12/boot-grub-rescue/" >/boot目录被清空下物理机无法开机的一次救援</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">10/11</span><a class="archive-post-title" href= "/2019/10/11/ansible-count-Idempotency/" >ansible数量限制上的幂等性</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">09/27</span><a class="archive-post-title" href= "/2019/09/27/consul-tls/" >高可用的SSL consul cluster实践</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">09/05</span><a class="archive-post-title" href= "/2019/09/05/prometheus-change-timezone/" >修改源码更改prometheus的时区问题</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">08/24</span><a class="archive-post-title" href= "/2019/08/24/gobot-build/" >gobot控制esp8266</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">08/06</span><a class="archive-post-title" href= "/2019/08/06/preseed/" >ubuntu preseed无人应答安装</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">07/14</span><a class="archive-post-title" href= "/2019/07/14/chromedp/" >golang headless browser包chromedp初探</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">07/08</span><a class="archive-post-title" href= "/2019/07/08/nodeport-err/" >为什么我不用nodePort之偶然中奖几率</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">07/07</span><a class="archive-post-title" href= "/2019/07/07/golang-http/" >golang的net/http包的客户端简单科普</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">06/26</span><a class="archive-post-title" href= "/2019/06/26/uefi-pxe/" >uefi模式下docker+交换机部署pxe批量安装</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">06/23</span><a class="archive-post-title" href= "/2019/06/23/autoInstallServer/" >拟定excel表格服务器自动按照表格配置信息和安装的实现过程</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">06/12</span><a class="archive-post-title" href= "/2019/06/12/CLP/" >SMASH CLP的一些笔记</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">06/02</span><a class="archive-post-title" href= "/2019/06/02/cobra/" >golang cobra的一些笔记</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/28</span><a class="archive-post-title" href= "/2019/04/28/k8s-java-start-time-not-same/" >闲谈线上俩k8s环境同等limits下pod启动时间不一样解决过程</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/22</span><a class="archive-post-title" href= "/2019/03/22/k8s-controller-error/" >一次kube-controller-manager的bug导致的线上无法调度处理过程</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/15</span><a class="archive-post-title" href= "/2019/03/15/flannel-bin/" >不走etcd v2 api下二进制跑flannel的总结</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/11</span><a class="archive-post-title" href= "/2019/03/11/k8s-ha/" >k8s高可用涉及到ip填写的相关配置和一些坑</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/03</span><a class="archive-post-title" href= "/2019/03/03/kubernetes-1-13-4/" >二进制部署Kubernetes v1.13.12 HA可选</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">02/19</span><a class="archive-post-title" href= "/2019/02/19/jira-confluence/" >docker部署jira(8.0.0)和confluence(6.14.1)</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">02/12</span><a class="archive-post-title" href= "/2019/02/12/dashboard/" >通用的dashboard部署和tls，SSL相关部署</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">01/30</span><a class="archive-post-title" href= "/2019/01/30/fstab/" >fstab与systemd.mount自动挂载的一点研究和见解</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">01/22</span><a class="archive-post-title" href= "/2019/01/22/proxmox-cloud-init/" >proxmox里使用cloud-init和一些笔记</a>
        </li>
    
    
    
    
    
        </ul>
    
    <div class="archive-year"> 2018 </div>
    <ul class="year-list">
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">12/04</span><a class="archive-post-title" href= "/2018/12/04/black-box-exporter/" >prometheus的黑盒监控</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">11/24</span><a class="archive-post-title" href= "/2018/11/24/how-to-use-kubeadm/" >对于初入k8s和kubeadm的一些建议</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">11/06</span><a class="archive-post-title" href= "/2018/11/06/onlyoffice/" >一次docker镜像的解耦--onlyoffice</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">11/05</span><a class="archive-post-title" href= "/2018/11/05/10chars/" >记录一次十字符病毒清理过程</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">10/27</span><a class="archive-post-title" href= "/2018/10/27/create-kubeconfig/" >生成kubeconfig常规的两种方法</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">10/12</span><a class="archive-post-title" href= "/2018/10/12/prometheus-operator/" >全手动部署prometheus-operator监控K8S集群以及一些坑</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">10/06</span><a class="archive-post-title" href= "/2018/10/06/IngressController/" >IngressController使用和它的高可用落地</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">09/24</span><a class="archive-post-title" href= "/2018/09/24/k8s-some-vpc-cluster/" >跨VPC或者跨云供应商搭建K8S集群正确姿势</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">09/18</span><a class="archive-post-title" href= "/2018/09/18/kubernetes-1-11-x-bin/" >二进制部署Kubernetes v1.11.x(1.12.x) HA可选</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">08/03</span><a class="archive-post-title" href= "/2018/08/03/Kubernetes_install_1.11.1/" >Kubernetes v1.11.x HA全手动苦工安装教学</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">07/18</span><a class="archive-post-title" href= "/2018/07/18/ecs-vip/" >基于openstack的ecs上使用VIP</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">07/08</span><a class="archive-post-title" href= "/2018/07/08/travis-sync-gcr-io/" >利用travis同步gcr.io镜像到dockerhub</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">06/25</span><a class="archive-post-title" href= "/2018/06/25/etcd-error/" >记录一次线上k8s节点故障</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">06/03</span><a class="archive-post-title" href= "/2018/06/03/kubernetes-s-job/" >kubernetes's Job总结和实战以及坑</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">06/02</span><a class="archive-post-title" href= "/2018/06/02/kubernetes-nodeSelector/" >kubernetes的PodAffinity的不解</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">05/05</span><a class="archive-post-title" href= "/2018/05/05/Kubernetes_install/" >[转载+修正]Kubernetes v1.10.x HA全手动苦工安装教学</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/29</span><a class="archive-post-title" href= "/2018/04/29/kubernetes-configMap-mount/" >kubernetes的configMap文件挂载不同的路径且不覆盖目录的解决方法</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/18</span><a class="archive-post-title" href= "/2018/03/18/keepalived-Heartbeat-use-mg-net/" >使用管理网当作业务网keepalived VIP的心跳线</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">02/05</span><a class="archive-post-title" href= "/2018/02/05/docker-image-can-t-rm/" >docker无法删除掉镜像的解决方法</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">01/20</span><a class="archive-post-title" href= "/2018/01/20/docker-rm%E7%9A%84%E6%B3%A8%E6%84%8F%E7%82%B9/" >慎用docker的--rm选项!!!</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">01/10</span><a class="archive-post-title" href= "/2018/01/10/docker%E7%9A%84%E4%B8%80%E4%BA%9B%E6%A6%82%E5%BF%B5/" >docker的一些概念</a>
        </li>
    
    
    
    
    
        </ul>
    
    <div class="archive-year"> 2017 </div>
    <ul class="year-list">
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">12/24</span><a class="archive-post-title" href= "/2017/12/24/docker%E5%AE%B9%E5%99%A8%E8%AE%BF%E9%97%AE%E5%AE%BF%E4%B8%BB%E6%9C%BA/" >docker容器访问宿主机</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">12/23</span><a class="archive-post-title" href= "/2017/12/23/docker%E5%AE%B9%E5%99%A8%E7%BD%91%E7%BB%9C%E4%BA%92%E8%81%94/" >docker容器网络互联</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">07/25</span><a class="archive-post-title" href= "/2017/07/25/linux-bridge/" >centos桥接测试</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">07/05</span><a class="archive-post-title" href= "/2017/07/05/centos7-some-mirror/" >centos7 的一些常见软件的安装 mirror</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">06/26</span><a class="archive-post-title" href= "/2017/06/26/lua-list-all-upsteam/" >lua列出所有upsteam</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">06/03</span><a class="archive-post-title" href= "/2017/06/03/bash-complete/" >bash自定义补全</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">05/25</span><a class="archive-post-title" href= "/2017/05/25/shell%E8%84%9A%E6%9C%AC%E7%9A%84%E9%80%89%E9%A1%B9%E5%A4%84%E7%90%86/" >shell脚本的选项和参数处理</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">05/12</span><a class="archive-post-title" href= "/2017/05/12/ssh-trust/" >ssh互信</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">05/06</span><a class="archive-post-title" href= "/2017/05/06/shell%E5%BF%AB%E6%8D%B7%E9%94%AE%E6%8F%90%E5%8D%87%E6%95%88%E7%8E%87/" >shell利用快捷键提升命令输入和编辑</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/29</span><a class="archive-post-title" href= "/2017/04/29/zabbixsetup/" >个人zabbix安装和坑的解决</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/26</span><a class="archive-post-title" href= "/2017/04/26/%E6%AD%A3%E5%88%99%E9%9B%B6%E5%AE%BD%E6%96%AD%E8%A8%80%E7%9A%84%E4%B8%80%E4%B8%AA%E6%B3%A8%E6%84%8F%E7%82%B9/" >正则零宽断言的一个注意点</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/25</span><a class="archive-post-title" href= "/2017/04/25/%E8%BD%AC%E8%BD%BD-awk%E4%B8%ADRS-OFS-RS-ORS%E5%8C%BA%E5%88%AB%E4%BA%8E%E8%81%94%E7%B3%BB/" >[转载]awk中RS,ORS,FS,OFS区别于联系</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/20</span><a class="archive-post-title" href= "/2017/04/20/lvm-practice/" >记录LVM和raid的练习</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/17</span><a class="archive-post-title" href= "/2017/04/17/iot/" >分享下自己做的外网控制硬件</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/15</span><a class="archive-post-title" href= "/2017/04/15/shell_process/" >shell多进程并发执行</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/15</span><a class="archive-post-title" href= "/2017/04/15/shellsubstring/" >shell的字符串截取</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/11</span><a class="archive-post-title" href= "/2017/04/11/8266hexdownload/" >8266模块的烧写和sdk的坑</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/09</span><a class="archive-post-title" href= "/2017/04/09/armlnmp/" >安卓安装linux并且源码编译安装搭建lnmp的坑和总结</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">04/03</span><a class="archive-post-title" href= "/2017/04/03/bond/" >centos配置bond</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/23</span><a class="archive-post-title" href= "/2017/03/23/check-dhcp-or-static/" >判断是否是 dhcp 获取ip的一个手段</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/20</span><a class="archive-post-title" href= "/2017/03/20/ftp-install/" >vsftpd虚拟用户简单部署</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">03/15</span><a class="archive-post-title" href= "/2017/03/15/lnmp/" >源码编译安装lnmp</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">02/26</span><a class="archive-post-title" href= "/2017/02/26/ad/" >Altium Designer里走线开窗和挖除铺铜还有一些技巧</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">02/12</span><a class="archive-post-title" href= "/2017/02/12/wx00/" >微信公众号接入自己服务器</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">02/02</span><a class="archive-post-title" href= "/2017/02/02/lamp/" >lamp环境搭建总结</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">01/08</span><a class="archive-post-title" href= "/2017/01/08/tuling-wx/" >微信公众号接入图灵机器人api</a>
        </li>
    
    
    
    
    
        </ul>
    
    <div class="archive-year"> 2016 </div>
    <ul class="year-list">
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">11/13</span><a class="archive-post-title" href= "/2016/11/13/cad/" >cad</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">10/30</span><a class="archive-post-title" href= "/2016/10/30/20161030/" >记录下自己制作的led-vu</a>
        </li>
    
    
        <li class="archive-post-item">
            <span class="archive-post-date">10/28</span><a class="archive-post-title" href= "/2016/10/28/hello/" >hello world</a>
        </li>
    
    </div>
  </div>
        <div class="sidebar-panel-tags">
    <div class="sidebar-tags-name">
    
        <span class="sidebar-tag-name" data-tags="diy"><span class="iconfont-archer">&#xe606;</span>diy</span>
    
        <span class="sidebar-tag-name" data-tags="8266"><span class="iconfont-archer">&#xe606;</span>8266</span>
    
        <span class="sidebar-tag-name" data-tags="总结"><span class="iconfont-archer">&#xe606;</span>总结</span>
    
        <span class="sidebar-tag-name" data-tags="ipmi"><span class="iconfont-archer">&#xe606;</span>ipmi</span>
    
        <span class="sidebar-tag-name" data-tags="CLP"><span class="iconfont-archer">&#xe606;</span>CLP</span>
    
        <span class="sidebar-tag-name" data-tags="k8s"><span class="iconfont-archer">&#xe606;</span>k8s</span>
    
        <span class="sidebar-tag-name" data-tags="ingress"><span class="iconfont-archer">&#xe606;</span>ingress</span>
    
        <span class="sidebar-tag-name" data-tags="Mismatch"><span class="iconfont-archer">&#xe606;</span>Mismatch</span>
    
        <span class="sidebar-tag-name" data-tags="Altium Designer"><span class="iconfont-archer">&#xe606;</span>Altium Designer</span>
    
        <span class="sidebar-tag-name" data-tags="ansible"><span class="iconfont-archer">&#xe606;</span>ansible</span>
    
        <span class="sidebar-tag-name" data-tags="consul"><span class="iconfont-archer">&#xe606;</span>consul</span>
    
        <span class="sidebar-tag-name" data-tags="lnmp"><span class="iconfont-archer">&#xe606;</span>lnmp</span>
    
        <span class="sidebar-tag-name" data-tags="安卓"><span class="iconfont-archer">&#xe606;</span>安卓</span>
    
        <span class="sidebar-tag-name" data-tags="initrd"><span class="iconfont-archer">&#xe606;</span>initrd</span>
    
        <span class="sidebar-tag-name" data-tags="grub"><span class="iconfont-archer">&#xe606;</span>grub</span>
    
        <span class="sidebar-tag-name" data-tags="raid"><span class="iconfont-archer">&#xe606;</span>raid</span>
    
        <span class="sidebar-tag-name" data-tags="Linux"><span class="iconfont-archer">&#xe606;</span>Linux</span>
    
        <span class="sidebar-tag-name" data-tags="kernel"><span class="iconfont-archer">&#xe606;</span>kernel</span>
    
        <span class="sidebar-tag-name" data-tags="prometheus"><span class="iconfont-archer">&#xe606;</span>prometheus</span>
    
        <span class="sidebar-tag-name" data-tags="exporter"><span class="iconfont-archer">&#xe606;</span>exporter</span>
    
        <span class="sidebar-tag-name" data-tags="boot"><span class="iconfont-archer">&#xe606;</span>boot</span>
    
        <span class="sidebar-tag-name" data-tags="cad"><span class="iconfont-archer">&#xe606;</span>cad</span>
    
        <span class="sidebar-tag-name" data-tags="centos6"><span class="iconfont-archer">&#xe606;</span>centos6</span>
    
        <span class="sidebar-tag-name" data-tags="golang"><span class="iconfont-archer">&#xe606;</span>golang</span>
    
        <span class="sidebar-tag-name" data-tags="chromedp"><span class="iconfont-archer">&#xe606;</span>chromedp</span>
    
        <span class="sidebar-tag-name" data-tags="cobra"><span class="iconfont-archer">&#xe606;</span>cobra</span>
    
        <span class="sidebar-tag-name" data-tags="docker"><span class="iconfont-archer">&#xe606;</span>docker</span>
    
        <span class="sidebar-tag-name" data-tags="Dockerfile"><span class="iconfont-archer">&#xe606;</span>Dockerfile</span>
    
        <span class="sidebar-tag-name" data-tags="keepavlied"><span class="iconfont-archer">&#xe606;</span>keepavlied</span>
    
        <span class="sidebar-tag-name" data-tags="etcd"><span class="iconfont-archer">&#xe606;</span>etcd</span>
    
        <span class="sidebar-tag-name" data-tags="flannel"><span class="iconfont-archer">&#xe606;</span>flannel</span>
    
        <span class="sidebar-tag-name" data-tags="cifs"><span class="iconfont-archer">&#xe606;</span>cifs</span>
    
        <span class="sidebar-tag-name" data-tags="ftp"><span class="iconfont-archer">&#xe606;</span>ftp</span>
    
        <span class="sidebar-tag-name" data-tags="go mod"><span class="iconfont-archer">&#xe606;</span>go mod</span>
    
        <span class="sidebar-tag-name" data-tags="gobot"><span class="iconfont-archer">&#xe606;</span>gobot</span>
    
        <span class="sidebar-tag-name" data-tags="esp8266"><span class="iconfont-archer">&#xe606;</span>esp8266</span>
    
        <span class="sidebar-tag-name" data-tags="http"><span class="iconfont-archer">&#xe606;</span>http</span>
    
        <span class="sidebar-tag-name" data-tags="hello world"><span class="iconfont-archer">&#xe606;</span>hello world</span>
    
        <span class="sidebar-tag-name" data-tags="mqtt"><span class="iconfont-archer">&#xe606;</span>mqtt</span>
    
        <span class="sidebar-tag-name" data-tags="原创"><span class="iconfont-archer">&#xe606;</span>原创</span>
    
        <span class="sidebar-tag-name" data-tags="jira"><span class="iconfont-archer">&#xe606;</span>jira</span>
    
        <span class="sidebar-tag-name" data-tags="confluence"><span class="iconfont-archer">&#xe606;</span>confluence</span>
    
        <span class="sidebar-tag-name" data-tags="kube-controller-manager"><span class="iconfont-archer">&#xe606;</span>kube-controller-manager</span>
    
        <span class="sidebar-tag-name" data-tags="java"><span class="iconfont-archer">&#xe606;</span>java</span>
    
        <span class="sidebar-tag-name" data-tags="springboot"><span class="iconfont-archer">&#xe606;</span>springboot</span>
    
        <span class="sidebar-tag-name" data-tags="kubeadm"><span class="iconfont-archer">&#xe606;</span>kubeadm</span>
    
        <span class="sidebar-tag-name" data-tags="ConfigMap"><span class="iconfont-archer">&#xe606;</span>ConfigMap</span>
    
        <span class="sidebar-tag-name" data-tags="PodAffinity"><span class="iconfont-archer">&#xe606;</span>PodAffinity</span>
    
        <span class="sidebar-tag-name" data-tags="lamp"><span class="iconfont-archer">&#xe606;</span>lamp</span>
    
        <span class="sidebar-tag-name" data-tags="nginx"><span class="iconfont-archer">&#xe606;</span>nginx</span>
    
        <span class="sidebar-tag-name" data-tags="microsoft"><span class="iconfont-archer">&#xe606;</span>microsoft</span>
    
        <span class="sidebar-tag-name" data-tags="graph"><span class="iconfont-archer">&#xe606;</span>graph</span>
    
        <span class="sidebar-tag-name" data-tags="onedrive"><span class="iconfont-archer">&#xe606;</span>onedrive</span>
    
        <span class="sidebar-tag-name" data-tags="nodeport"><span class="iconfont-archer">&#xe606;</span>nodeport</span>
    
        <span class="sidebar-tag-name" data-tags="preseed"><span class="iconfont-archer">&#xe606;</span>preseed</span>
    
        <span class="sidebar-tag-name" data-tags="timezone"><span class="iconfont-archer">&#xe606;</span>timezone</span>
    
        <span class="sidebar-tag-name" data-tags="operator"><span class="iconfont-archer">&#xe606;</span>operator</span>
    
        <span class="sidebar-tag-name" data-tags="openstack"><span class="iconfont-archer">&#xe606;</span>openstack</span>
    
        <span class="sidebar-tag-name" data-tags="cloud-init"><span class="iconfont-archer">&#xe606;</span>cloud-init</span>
    
        <span class="sidebar-tag-name" data-tags="linux"><span class="iconfont-archer">&#xe606;</span>linux</span>
    
        <span class="sidebar-tag-name" data-tags="shell"><span class="iconfont-archer">&#xe606;</span>shell</span>
    
        <span class="sidebar-tag-name" data-tags="bash"><span class="iconfont-archer">&#xe606;</span>bash</span>
    
        <span class="sidebar-tag-name" data-tags="ssh"><span class="iconfont-archer">&#xe606;</span>ssh</span>
    
        <span class="sidebar-tag-name" data-tags="suse"><span class="iconfont-archer">&#xe606;</span>suse</span>
    
        <span class="sidebar-tag-name" data-tags="dockerhub"><span class="iconfont-archer">&#xe606;</span>dockerhub</span>
    
        <span class="sidebar-tag-name" data-tags="gcr.io"><span class="iconfont-archer">&#xe606;</span>gcr.io</span>
    
        <span class="sidebar-tag-name" data-tags="微信"><span class="iconfont-archer">&#xe606;</span>微信</span>
    
        <span class="sidebar-tag-name" data-tags="api"><span class="iconfont-archer">&#xe606;</span>api</span>
    
        <span class="sidebar-tag-name" data-tags="tftp"><span class="iconfont-archer">&#xe606;</span>tftp</span>
    
        <span class="sidebar-tag-name" data-tags="zabbix"><span class="iconfont-archer">&#xe606;</span>zabbix</span>
    
        <span class="sidebar-tag-name" data-tags="正则"><span class="iconfont-archer">&#xe606;</span>正则</span>
    
        <span class="sidebar-tag-name" data-tags="awk"><span class="iconfont-archer">&#xe606;</span>awk</span>
    
        <span class="sidebar-tag-name" data-tags="N1"><span class="iconfont-archer">&#xe606;</span>N1</span>
    
        <span class="sidebar-tag-name" data-tags="openwrt"><span class="iconfont-archer">&#xe606;</span>openwrt</span>
    
        <span class="sidebar-tag-name" data-tags="go"><span class="iconfont-archer">&#xe606;</span>go</span>
    
        <span class="sidebar-tag-name" data-tags="63s"><span class="iconfont-archer">&#xe606;</span>63s</span>
    
        <span class="sidebar-tag-name" data-tags="timeout"><span class="iconfont-archer">&#xe606;</span>timeout</span>
    
        <span class="sidebar-tag-name" data-tags="host-gw"><span class="iconfont-archer">&#xe606;</span>host-gw</span>
    
        <span class="sidebar-tag-name" data-tags="kubeconfig"><span class="iconfont-archer">&#xe606;</span>kubeconfig</span>
    
        <span class="sidebar-tag-name" data-tags="x86"><span class="iconfont-archer">&#xe606;</span>x86</span>
    
        <span class="sidebar-tag-name" data-tags="Prometheus"><span class="iconfont-archer">&#xe606;</span>Prometheus</span>
    
        <span class="sidebar-tag-name" data-tags="openshift"><span class="iconfont-archer">&#xe606;</span>openshift</span>
    
        <span class="sidebar-tag-name" data-tags="ocp"><span class="iconfont-archer">&#xe606;</span>ocp</span>
    
        <span class="sidebar-tag-name" data-tags="Kylin"><span class="iconfont-archer">&#xe606;</span>Kylin</span>
    
        <span class="sidebar-tag-name" data-tags="uos"><span class="iconfont-archer">&#xe606;</span>uos</span>
    
        <span class="sidebar-tag-name" data-tags="vip"><span class="iconfont-archer">&#xe606;</span>vip</span>
    
        <span class="sidebar-tag-name" data-tags="wireguard"><span class="iconfont-archer">&#xe606;</span>wireguard</span>
    
        <span class="sidebar-tag-name" data-tags="swap"><span class="iconfont-archer">&#xe606;</span>swap</span>
    
        <span class="sidebar-tag-name" data-tags="hang"><span class="iconfont-archer">&#xe606;</span>hang</span>
    
        <span class="sidebar-tag-name" data-tags="coredns"><span class="iconfont-archer">&#xe606;</span>coredns</span>
    
    </div>
    <div class="iconfont-archer sidebar-tags-empty">&#xe678;</div>
    <div class="tag-load-fail" style="display: none; color: #ccc; font-size: 0.6rem;">
    缺失模块。<br/>
    1、请确保node版本大于6.2<br/>
    2、在博客根目录（注意不是archer根目录）执行以下命令：<br/>
    <span style="color: #f75357; font-size: 1rem; line-height: 2rem;">npm i hexo-generator-json-content --save</span><br/>
    3、在根目录_config.yml里添加配置：
    <pre style="color: #787878; font-size: 0.6rem;">
jsonContent:
  meta: false
  pages: false
  posts:
    title: true
    date: true
    path: true
    text: false
    raw: false
    content: false
    slug: false
    updated: false
    comments: false
    link: false
    permalink: false
    excerpt: false
    categories: true
    tags: true</pre>
    </div> 
    <div class="sidebar-tags-list"></div>
</div>
        <div class="sidebar-panel-categories">
    <div class="sidebar-categories-name">
    
        <span class="sidebar-category-name" data-categories="日志"><span class="iconfont-archer">&#xe60a;</span>日志</span>
    
        <span class="sidebar-category-name" data-categories="ipmi"><span class="iconfont-archer">&#xe60a;</span>ipmi</span>
    
        <span class="sidebar-category-name" data-categories="kubernetes"><span class="iconfont-archer">&#xe60a;</span>kubernetes</span>
    
        <span class="sidebar-category-name" data-categories="日志/闲搞"><span class="iconfont-archer">&#xe60a;</span>日志/闲搞</span>
    
        <span class="sidebar-category-name" data-categories="日志/心得"><span class="iconfont-archer">&#xe60a;</span>日志/心得</span>
    
        <span class="sidebar-category-name" data-categories="ansible"><span class="iconfont-archer">&#xe60a;</span>ansible</span>
    
        <span class="sidebar-category-name" data-categories="pxe"><span class="iconfont-archer">&#xe60a;</span>pxe</span>
    
        <span class="sidebar-category-name" data-categories="Linux"><span class="iconfont-archer">&#xe60a;</span>Linux</span>
    
        <span class="sidebar-category-name" data-categories="prometheus"><span class="iconfont-archer">&#xe60a;</span>prometheus</span>
    
        <span class="sidebar-category-name" data-categories="boot"><span class="iconfont-archer">&#xe60a;</span>boot</span>
    
        <span class="sidebar-category-name" data-categories="kubernetes/kubelet"><span class="iconfont-archer">&#xe60a;</span>kubernetes/kubelet</span>
    
        <span class="sidebar-category-name" data-categories="日志/Auto-cad"><span class="iconfont-archer">&#xe60a;</span>日志/Auto-cad</span>
    
        <span class="sidebar-category-name" data-categories="golang"><span class="iconfont-archer">&#xe60a;</span>golang</span>
    
        <span class="sidebar-category-name" data-categories="consul"><span class="iconfont-archer">&#xe60a;</span>consul</span>
    
        <span class="sidebar-category-name" data-categories="ansible/心得"><span class="iconfont-archer">&#xe60a;</span>ansible/心得</span>
    
        <span class="sidebar-category-name" data-categories="pxe/raid"><span class="iconfont-archer">&#xe60a;</span>pxe/raid</span>
    
        <span class="sidebar-category-name" data-categories="Linux/boot"><span class="iconfont-archer">&#xe60a;</span>Linux/boot</span>
    
        <span class="sidebar-category-name" data-categories="boot/grub"><span class="iconfont-archer">&#xe60a;</span>boot/grub</span>
    
        <span class="sidebar-category-name" data-categories="Linux/centos6"><span class="iconfont-archer">&#xe60a;</span>Linux/centos6</span>
    
        <span class="sidebar-category-name" data-categories="pxe/raid/kickstart"><span class="iconfont-archer">&#xe60a;</span>pxe/raid/kickstart</span>
    
        <span class="sidebar-category-name" data-categories="Linux/centos6/boot"><span class="iconfont-archer">&#xe60a;</span>Linux/centos6/boot</span>
    
        <span class="sidebar-category-name" data-categories="日志/容器"><span class="iconfont-archer">&#xe60a;</span>日志/容器</span>
    
        <span class="sidebar-category-name" data-categories="kubernetes/docker"><span class="iconfont-archer">&#xe60a;</span>kubernetes/docker</span>
    
        <span class="sidebar-category-name" data-categories="docker"><span class="iconfont-archer">&#xe60a;</span>docker</span>
    
        <span class="sidebar-category-name" data-categories="容器"><span class="iconfont-archer">&#xe60a;</span>容器</span>
    
        <span class="sidebar-category-name" data-categories="kubernetes/docker/panic"><span class="iconfont-archer">&#xe60a;</span>kubernetes/docker/panic</span>
    
        <span class="sidebar-category-name" data-categories="openstack"><span class="iconfont-archer">&#xe60a;</span>openstack</span>
    
        <span class="sidebar-category-name" data-categories="fstab"><span class="iconfont-archer">&#xe60a;</span>fstab</span>
    
        <span class="sidebar-category-name" data-categories="vsftp"><span class="iconfont-archer">&#xe60a;</span>vsftp</span>
    
        <span class="sidebar-category-name" data-categories="gobot"><span class="iconfont-archer">&#xe60a;</span>gobot</span>
    
        <span class="sidebar-category-name" data-categories="golang/http"><span class="iconfont-archer">&#xe60a;</span>golang/http</span>
    
        <span class="sidebar-category-name" data-categories="日志/闲聊"><span class="iconfont-archer">&#xe60a;</span>日志/闲聊</span>
    
        <span class="sidebar-category-name" data-categories="kubernetes/kube-controller-manager"><span class="iconfont-archer">&#xe60a;</span>kubernetes/kube-controller-manager</span>
    
        <span class="sidebar-category-name" data-categories="kubernetes/kubeadm"><span class="iconfont-archer">&#xe60a;</span>kubernetes/kubeadm</span>
    
        <span class="sidebar-category-name" data-categories="kubernetes/k8s"><span class="iconfont-archer">&#xe60a;</span>kubernetes/k8s</span>
    
        <span class="sidebar-category-name" data-categories="kubernetes/Job"><span class="iconfont-archer">&#xe60a;</span>kubernetes/Job</span>
    
        <span class="sidebar-category-name" data-categories="lua"><span class="iconfont-archer">&#xe60a;</span>lua</span>
    
        <span class="sidebar-category-name" data-categories="microsoft"><span class="iconfont-archer">&#xe60a;</span>microsoft</span>
    
        <span class="sidebar-category-name" data-categories="preseed"><span class="iconfont-archer">&#xe60a;</span>preseed</span>
    
        <span class="sidebar-category-name" data-categories="prometheus/golang"><span class="iconfont-archer">&#xe60a;</span>prometheus/golang</span>
    
        <span class="sidebar-category-name" data-categories="kubernetes/prometheus"><span class="iconfont-archer">&#xe60a;</span>kubernetes/prometheus</span>
    
        <span class="sidebar-category-name" data-categories="proxmox"><span class="iconfont-archer">&#xe60a;</span>proxmox</span>
    
        <span class="sidebar-category-name" data-categories="日志/总结"><span class="iconfont-archer">&#xe60a;</span>日志/总结</span>
    
        <span class="sidebar-category-name" data-categories="microsoft/graph"><span class="iconfont-archer">&#xe60a;</span>microsoft/graph</span>
    
        <span class="sidebar-category-name" data-categories="microsoft/graph/onedrive"><span class="iconfont-archer">&#xe60a;</span>microsoft/graph/onedrive</span>
    
        <span class="sidebar-category-name" data-categories="boot/grub/suse"><span class="iconfont-archer">&#xe60a;</span>boot/grub/suse</span>
    
        <span class="sidebar-category-name" data-categories="CI"><span class="iconfont-archer">&#xe60a;</span>CI</span>
    
        <span class="sidebar-category-name" data-categories="pxe/docker"><span class="iconfont-archer">&#xe60a;</span>pxe/docker</span>
    
        <span class="sidebar-category-name" data-categories="日志/运维"><span class="iconfont-archer">&#xe60a;</span>日志/运维</span>
    
        <span class="sidebar-category-name" data-categories="CI/travis"><span class="iconfont-archer">&#xe60a;</span>CI/travis</span>
    
        <span class="sidebar-category-name" data-categories="日志/技巧"><span class="iconfont-archer">&#xe60a;</span>日志/技巧</span>
    
        <span class="sidebar-category-name" data-categories="日志/LVM"><span class="iconfont-archer">&#xe60a;</span>日志/LVM</span>
    
        <span class="sidebar-category-name" data-categories="pxe/docker/kickstart"><span class="iconfont-archer">&#xe60a;</span>pxe/docker/kickstart</span>
    
        <span class="sidebar-category-name" data-categories="日志/LVM/raid"><span class="iconfont-archer">&#xe60a;</span>日志/LVM/raid</span>
    
        <span class="sidebar-category-name" data-categories="golang/version"><span class="iconfont-archer">&#xe60a;</span>golang/version</span>
    
        <span class="sidebar-category-name" data-categories="k8s"><span class="iconfont-archer">&#xe60a;</span>k8s</span>
    
        <span class="sidebar-category-name" data-categories="k8s/vxlan"><span class="iconfont-archer">&#xe60a;</span>k8s/vxlan</span>
    
        <span class="sidebar-category-name" data-categories="go"><span class="iconfont-archer">&#xe60a;</span>go</span>
    
        <span class="sidebar-category-name" data-categories="go/Prometheus"><span class="iconfont-archer">&#xe60a;</span>go/Prometheus</span>
    
        <span class="sidebar-category-name" data-categories="kubeconfig"><span class="iconfont-archer">&#xe60a;</span>kubeconfig</span>
    
        <span class="sidebar-category-name" data-categories="Prometheus"><span class="iconfont-archer">&#xe60a;</span>Prometheus</span>
    
        <span class="sidebar-category-name" data-categories="k8s/Kylin"><span class="iconfont-archer">&#xe60a;</span>k8s/Kylin</span>
    
        <span class="sidebar-category-name" data-categories="k8s/uos"><span class="iconfont-archer">&#xe60a;</span>k8s/uos</span>
    
        <span class="sidebar-category-name" data-categories="keepalived"><span class="iconfont-archer">&#xe60a;</span>keepalived</span>
    
        <span class="sidebar-category-name" data-categories="wireguard"><span class="iconfont-archer">&#xe60a;</span>wireguard</span>
    
        <span class="sidebar-category-name" data-categories="linux"><span class="iconfont-archer">&#xe60a;</span>linux</span>
    
        <span class="sidebar-category-name" data-categories="kubernetes/coredns"><span class="iconfont-archer">&#xe60a;</span>kubernetes/coredns</span>
    
        <span class="sidebar-category-name" data-categories="kubernetes/coredns/node-cache"><span class="iconfont-archer">&#xe60a;</span>kubernetes/coredns/node-cache</span>
    
        <span class="sidebar-category-name" data-categories="admission"><span class="iconfont-archer">&#xe60a;</span>admission</span>
    
        <span class="sidebar-category-name" data-categories="iptables"><span class="iconfont-archer">&#xe60a;</span>iptables</span>
    
        <span class="sidebar-category-name" data-categories="k8s/kmem"><span class="iconfont-archer">&#xe60a;</span>k8s/kmem</span>
    
    </div>
    <div class="iconfont-archer sidebar-categories-empty">&#xe678;</div>
    <div class="sidebar-categories-list"></div>
</div>
    </div>
</div> 
    <script>
    var siteMeta = {
        root: "/",
        author: "Zhangguanzhang"
    }
</script>
    <!-- CDN failover -->
    <script src="https://cdn.jsdelivr.net/npm/jquery@3.3.1/dist/jquery.min.js"></script>
    <script type="text/javascript">
        if (typeof window.$ === 'undefined')
        {
            console.warn('jquery load from jsdelivr failed, will load local script')
            document.write('<script src="/lib/jquery.min.js">\x3C/script>')
        }
    </script>
    <script src="/scripts/main.js"></script>
    <!-- algolia -->
    
    <!-- busuanzi  -->
    
    <script async src="//busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js"></script>
    
    <!-- CNZZ  -->
    
    </div>
    <!-- async load share.js -->
     
    </body>
</html>


