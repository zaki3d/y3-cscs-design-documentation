These are some of the common elements used throughout the app. Please refer to this documentation when creating/using UI elements for the app.

##Table of Contents
1. [Colors](#colors)
1. [Navigations](#navigations)
1. [Type](#type)
1. [Form Elements](#form-elements)
1. [Buttons and Switches](#buttons-switches)
1. [Tables](#tables)
1. [Tiers](#tiers)
1. [Alerts](#alerts)
1. [Dialogs](#dialogs)
1. [Themes](#themes)

##Colors<a name="#colors"></a>
These are the colors for the default theme of the app. For better consistency, colors used throughout the app should be strictly limited to the default palette below (unless a different theme is picked in which a different palette will be prepared).

#####Primary
1. ![](https://s3.amazonaws.com/f.cl.ly/items/33380H2L1L341q361s1I/col-pri-blue.png) `#4A90E2` - Royal Blue
1. ![](https://s3.amazonaws.com/f.cl.ly/items/1e0k320A1U1R0O0s3C1l/col-pri-smoke.png) `#F8F8F8` - White Smoke
1. ![](https://s3.amazonaws.com/f.cl.ly/items/2a1x1K1e1y280a2u163z/col-pri-black.png) `#000000` - Solid Black
1. ![](https://www.evernote.com/shard/s38/sh/5ba4ca93-99c8-419d-a05a-cfb21d16b1a5/23b7b06a7fd9c04bc80a179b3bed8cb3/deep/0/col-pri-white.png) `#FFFFFF` - White

#####Secondary
1. ![](https://s3.amazonaws.com/f.cl.ly/items/1W0u3q3D02180e250825/col-sec-blue-1.png) `#ECF8FE` - Alice Blue
1. ![](https://s3.amazonaws.com/f.cl.ly/items/1R232k2k3D432f0r3y2A/col-sec-blue-2.png) `#95C0F3` - Sky Blue
1. ![](https://s3.amazonaws.com/f.cl.ly/items/3N3K1o1j3g0v2W3F1b16/col-sec-yellow-1.png) `#FFEFBD` - Moccasin
1. ![](https://s3.amazonaws.com/f.cl.ly/items/0n0s3M1X1f0i3I2d0y2b/col-sec-yellow-2.png) `#F9D415` - Turbo
1. ![](https://s3.amazonaws.com/f.cl.ly/items/1H3F0O1t0X2w42191r1Q/col-sec-green-1.png) `#D7F6B4` - Snow Flurry
1. ![](https://s3.amazonaws.com/f.cl.ly/items/3R3E2c0y3n1B2a15060U/col-sec-green-2.png) `#99DD4F` - Conifer
1. ![](https://s3.amazonaws.com/f.cl.ly/items/3j0v0e0o1Q36061K0B3v/col-sec-red-1.png) `#FFD2D2` - Pink
1. ![](https://s3.amazonaws.com/f.cl.ly/items/0E3r1I1H2g3c00132109/col-sec-red-2.png) `#FF6666` - Bittersweet

#####Grey
1. ![](https://s3.amazonaws.com/f.cl.ly/items/2w1O3C113b3E2M1T3S0O/col-grey-1.png) `#999999` - Nobel Grey
1. ![](https://s3.amazonaws.com/f.cl.ly/items/182w0H2M350z0T411T1N/col-grey-2.png) `#DADADA` - Gainsboro Grey
1. ![](https://s3.amazonaws.com/f.cl.ly/items/0F331P2n3A3u2J392y12/col-grey-3.png) `#EEEEEE` - Cement Grey

#####Gradients
1. ![](https://s3.amazonaws.com/f.cl.ly/items/062M2K3M3F092R0G3G2s/col-grad-blue.png) `#1968C2(Top) - #095CBB(Bottom)` - Royal Blue Gradient
1. ![](https://s3.amazonaws.com/f.cl.ly/items/2L0I1A2r3o3V412D2N41/col-grad-grey-1.png) `#FFFFFF(Top) - #F8F8F8(Bottom)` - Grey Gradient (Up)
1. ![](https://s3.amazonaws.com/f.cl.ly/items/1f3H3w3d431f3P1e0i3j/col-grad-grey-2.png) `#F0F0F0(Top) - #FAFAFA(Bottom)` - Grey Gradient (Down)

##Navigations<a name="#navigations"></a>
1. Main Navigation
	![](https://www.evernote.com/shard/s38/sh/53cbd344-b125-489f-8756-070f11159255/28ecf15c224de77dfdbda5f84a63d752/deep/0/nav-main.png)
	HTML:
	```html
	<div class="nav-main">
		<ul>
			<li><a href="#">Link Item</a></li>
			<li><a href="#">Link Item</a></li>
			<li><a href="#">Link Item</a></li>
		</ul>
	</div>
	```
	CSS:
	```css
	.nav-main {
		background-image: linear-gradient(-180deg, #1968C2 0%, #095CBB 100%);
		padding: 20px 24px;
		box-shadow: 0px 1px 2px 0px rgba(0,0,0,0.3);
	}
	.nav-main ul {
		padding: 0;
		margin: 0;
		list-style-type: none;
	}
	.nav-main ul li {
		padding: 0 14px;
		display: inline;
	}
	.nav-main ul li:first-child {
		padding-left: 0;
	}
	.nav-main ul li a {
		color: rgb(112,161,216);
		color: rgba(255,255,255,0.4);
		text-decoration: none;
	}
	.nav-main ul li a:hover, .nav-main ul li a:active {
		color: #FFFFFF;
	}
	```

1. Local Navigation
	![](https://www.evernote.com/shard/s38/sh/29238709-8f7b-4c5c-8024-a20af9d7e762/224ccf83fbe964b053c2ce5ba45d899f/deep/0/nav-local.png)
	HTML:
	```html
	<div class="nav-local">
		<ul>
			<li><a href="#">Link Item</a></li>
			<li><a href="#">Link Item</a></li>
			<li><a href="#">Link Item</a></li>
		</ul>
	</div>
	```
	CSS:
	```css
	.nav-local {
		padding: 14px;
		border-bottom: 1px solid #DADADA;
	}
	.nav-local ul {
		padding: 0;
		margin: 0;
		list-style-type: none;
	}
	.nav-local ul li {
		padding: 0 8px;
		display: inline;
	}
	.nav-local ul li:first-child {
		padding-left: 0;
	}
	.nav-local ul li a {
		padding: 4px 8px;
		background: #FFFFFF;
		border-radius: 2px;
		color: #000000;
		text-decoration: none;
	}
	.nav-local ul li a:hover {
		padding: 4px 8px;
		background: #EEEEEE;
		border-radius: 2px;
	}
	.nav-local ul li a:active {
		padding: 4px 8px;
		background: #ECF8FE;
		border-radius: 2px;
		color: #4A90E2;
	}
	```

##Type<a name="#type"></a>
####Header type
1. ![](https://www.evernote.com/shard/s38/sh/b57ba69e-f2d6-4841-b2a9-fab300502076/44ef605018ef518cfbd63b58c53edeb0/deep/0/type-header-1.png)
	```css
	h1 {font-size: 36px; color: #000000; line-height: 46px;}
	```

1. ![](https://www.evernote.com/shard/s38/sh/a1c86f00-4efb-497b-9d27-959a3c04fde8/171e4f72bc48600e802813dfcfe596df/deep/0/type-header-2.png)
	```css
	h2 {font-size: 24px; color: #000000; line-height: 36px;}
	```

1. ![](https://www.evernote.com/shard/s38/sh/c2686a75-9188-496e-b704-8fc796355193/c3dfaf599b5fcb6a7651327657ce4622/deep/0/type-header-3.png)
	```css
	h3 {font-size: 21px; color: #000000; line-height: 28px;}
	```

1. ![](https://www.evernote.com/shard/s38/sh/214bb1e6-8ee1-44f8-b6bf-6d8b694544fc/bde5038f28f3c700ba5b58208ebcfdcc/deep/0/type-header-4.png)
	```css
	h4 {font-size: 14px; color: #000000; line-height: 24px;}
	```

1. ![](https://www.evernote.com/shard/s38/sh/1299409c-3f22-4fe4-b57a-f7c1af773f43/e070e5814d6f1251b35d01e75857956b/deep/0/type-header-4-link.png)
	```css
	h4 a {font-size: 14px; color: #4A90E2; line-height: 24px;}
	```

####Body type
1. ![](https://www.evernote.com/shard/s38/sh/6b639713-3af6-419b-ad97-362da8697982/62bd497acf708dad7139729aba96e1ec/deep/0/type-body-normal.png)
	```css
	p {font-size: 14px; color: #000000; line-height: 24px;}
	```

1. ![](https://www.evernote.com/shard/s38/sh/c286b1b1-71d3-4db8-baba-05ddda3d6cce/f77e7a4e0412f1bc02c09edd7708f8ce/deep/0/type-body-faded.png)
	```css
	p.faded {color: #999999;}
	```

1. ![](https://www.evernote.com/shard/s38/sh/086861ce-7cc3-44ab-af53-ce90d3cf9751/8e6413473a8c5390eac57811ab69a2c2/deep/0/type-body-link.png)
	```css
	p a {color: #4A90E2; text-decoration: none;}
	p a:hover {color: #095CBB;}
	```

####Small type
1. ![](https://www.evernote.com/shard/s38/sh/7dc00595-052e-4287-bd24-73facc8d50b7/ebdde91bce224a32492ecd6d83694f17/deep/0/type-small-normal.png)
	```css
	small {font-size: 12px; color: #999999; line-height: 16px;}
	```

1. ![](https://www.evernote.com/shard/s38/sh/baffe762-c2f9-4107-8560-35e879f97114/89e000c5e3ca723dce8c2c34f440bb8e/deep/0/type-small-link.png)
	```css
	small a {color: #4A90E2; text-decoration: none;}
	```

####Label type
1. ![](https://www.evernote.com/shard/s38/sh/0cd28b18-d542-4a9d-87ad-12139f585546/7b6f5428fae218785cc3bea0a1fb21ea/deep/0/type-label.png)
	```css
	label {font-size: 11px; color: #DADADA; line-height: 15px;}
	```

##Form Elements<a name="#form-elements"></a>


##Buttons and Switches<a name="#buttons-switches"></a>
##Tables<a name="#tables"></a>
##Tiers<a name="#tiers"></a>
##Alerts<a name="#alerts"></a>
Test

##Dialogs<a name="#dialogs"></a>
##Themes<a name="#themes"></a>