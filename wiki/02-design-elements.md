These are some of the common elements used throughout the app. Please refer to this documentation when creating/using UI elements for the app.

##Table of Contents
1. [Colors](#colors)
1. [Navigations](#navigations)
1. [Fonts](#fonts)
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
		color: rgb(112,161,216);
		color: rgba(255,255,255,0.4);
	}
	.nav-main ul {
		list-style-type: none;
	}
	.nav-main ul li {
		display: inline;
	}
	.nav-main ul li:hover, .nav-main ul li:active {
		color: #FFFFFF;
	}
	```

1. Local Navigation
	![](https://www.evernote.com/shard/s38/sh/29238709-8f7b-4c5c-8024-a20af9d7e762/224ccf83fbe964b053c2ce5ba45d899f/deep/0/nav-local.png)
	```css
		.nav-local {
			padding: 14px;
			border-bottom: 1px solid #DADADA;
			color: #000000;
		}

		.nav-local a:hover {
			background: #F8F8F8;
			padding: 4px 8px;
			border-radius: 2px;
			color: #000000;
		}

		.nav-local a:active {
		  background: #ECF8FE;
			padding: 4px 8px;
			border-radius: 2px;
			color: #4A90E2;
		}
	```

1. Local Navigation (with icons)
![](https://www.evernote.com/shard/s38/sh/85e7d348-ad7a-41b6-a9bb-7c6cb6b90f05/dde345a0277746fdab816164b0589ba8/deep/0/nav-local-icons.png)

##Fonts<a name="#fonts"></a>
##Form Elements<a name="#form-elements"></a>
##Buttons and Switches<a name="#buttons-switches"></a>
##Tables<a name="#tables"></a>
##Tiers<a name="#tiers"></a>
##Alerts<a name="#alerts"></a>
Test

##Dialogs<a name="#dialogs"></a>
##Themes<a name="#themes"></a>