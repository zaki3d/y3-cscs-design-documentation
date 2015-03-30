These are some of the common elements used throughout the app. Please refer to this documentation when creating/using UI elements for the app.

> *Disclaimer: Some of the html/css codes are extracted from Sketch and may be incomplete for implementation. They serve as a starting point for the front-end styling. Please update this documentation accordingly based on the final implementation.*


##Table of Contents
1. [Colors](#colors)
1. [Navigations](#navigations)
1. [Type](#type)
1. [Form Elements](#form-elements)
1. [Buttons and Switches](#buttons-switches)
1. [Tables](#tables)
1. [Alerts](#alerts)
1. [Dialogs](#dialogs)

##Colors<a name="#colors"></a>
These are the colors for the default theme of the app. For better consistency, colors used throughout the app should be strictly limited to the default palette below (unless a different theme is picked in which a different palette will be prepared).

#####Primary
1. ![](https://s3.amazonaws.com/f.cl.ly/items/33380H2L1L341q361s1I/col-pri-blue.png) `#4A90E2` - Royal Blue
1. ![](https://s3.amazonaws.com/f.cl.ly/items/1W0u3q3D02180e250825/col-sec-blue-1.png) `#ECF8FE` - Alice Blue (Complimentary)
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
		color: #000000;
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
		color: #000000;
		text-decoration: none;
	}
	.nav-local ul li a:hover {
		padding: 4px 8px;
		background: #EEEEEE;
		border-radius: 2px;
	}
	.nav-local ul li a.active {
		padding: 4px 8px;
		background: #ECF8FE;
		border-radius: 2px;
		color: #4A90E2;
	}
	.nav-local ul li a.active:hover {
		background: #ECF8FE;
		color: #4A90E2;
	}
	```

1. Tabs

	![](https://www.evernote.com/shard/s38/sh/55663fb0-8b9b-42f3-918a-bd62ff92a4c1/4ae23571f30d64029d85f8dadf1e45fd/deep/0/nav-tabs.png)

	CSS:

	```css
	.tabs	{
		padding: 8px 0;
		margin-top: 20px;
		border-bottom: 1px solid #DADADA;
	}
	.tabs ul {
		padding: 0;
		margin: 0;
		list-style-type: none;
	}
	.tabs ul a {
		text-decoration: none;
	}
	.tabs ul li {
		padding: 8px 14px;
		margin: 0 2px;
		background: #EDEDED;
		border: 1px solid #DADADA;
		-webkit-border-radius: 3px 3px 0 0;
		        border-radius: 3px 3px 0 0;
		color: #999999;
		display: inline;
	}
	.tabs ul li:hover {
		color: #000000;
	}
	.tabs ul li.active {
		background: #FFFFFF;
		border: 1px solid #DADADA;
		color: #000000;
		border-bottom: 1px solid #FFFFFF;
	}
	```

	For full implementation guide, please refer to [Bootstrap Tabs](http://getbootstrap.com/javascript/#tabs) for implementation guide.

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
	label {font-size: 11px; color: #DADADA; line-height: 15px; text-transform: uppercase;}
	```

##Form Elements<a name="#form-elements"></a>
####Input
1. Input label
	
	![](https://www.evernote.com/shard/s38/sh/0cd28b18-d542-4a9d-87ad-12139f585546/7b6f5428fae218785cc3bea0a1fb21ea/deep/0/type-label.png)
	
	Each field is usually preceded by a label. This is the default styling for all labels in a form.

	CSS:

	```css
	form label {
		font-size: 11px;
		color: #DADADA;
		line-height: 15px;
		text-transform: uppercase;
	}
	```

1. Input field (Normal & focused)

	![](https://www.evernote.com/shard/s38/sh/b5bb25f4-53f9-443b-9048-a351656edcae/47976092a89aa36f4b2661e961aeb71f/deep/0/form-input-empty.png)

	![](https://www.evernote.com/shard/s38/sh/40500d89-55ce-4365-9ea5-e6ea467012df/68a4bc2de5131ef79ee55e39bd82a5e8/deep/0/form-input-active-with-note.png)

	HTML:

	```html
	<form>
		<input type="text" placeholder="Input empty">
	</form>
	```

	CSS:

	```css
	form input:not([type=submit]):not([type=file]) {
		background: #F8F8F8;
		width: 100%;
		padding: 8px 14px;
		margin-top: 4px;
		margin-bottom: 10px;
		border: 1px solid #DADADA;
		box-shadow: inset 0px 1px 1px 0px rgba(0,0,0,0.06);
		border-radius: 2px;
		font-size: 14px;
		transition: box-shadow 0.3s, border 0.3s;
	}

	form input:not([type=submit]):not([type=file]):focus {
		outline: none;
		border: 1px solid #75B3FA;
		box-shadow: 0px 0px 3px 0px #CCDFF6, inset 0px 1px 1px 0px rgba(0,0,0,0.06);
	}
	```

1. Input field (Disabled)

	![](https://www.evernote.com/shard/s38/sh/ada4102c-047c-4ce1-8fa7-65a14c2cf1ab/44a0f238f2f3841710aafac2f9dc358c/deep/0/form-input-disabled.png)

	HTML:

	```html
	<form>
		<input type="text" placeholder="Input disabled" disabled>
	</form>
	```

	CSS:

	```css
	form input:not([type=submit]):not([type=file]):disabled {
		background: #F8F8F8;
		border: 1px solid #ECECEC;
		-webkit-box-shadow: none;
		box-shadow: none;
	}
	```

1. Input field (Invalid)

	![](https://www.evernote.com/shard/s38/sh/c14a6710-d68e-4ef7-9867-ccbc22d4de9b/8e4b22efb2e4def9b4bed9475eccb83f/deep/0/form-input-error-with-note.png)

	HTML:

	```html
	<form>
		<input type="text" placeholder="Input invalid">
	</form>
	```

	CSS:

	```css
	form input:not([type=submit]):not([type=file]):invalid {
		background: #FFF9F9;
		border: 1px solid #FB5E73;
		box-shadow: inset 0px 1px 1px 0px rgba(0,0,0,0.06);
		color: #FF6666;
	}
	```

<!-- 1. Input field with button

	![](https://www.evernote.com/shard/s38/sh/1b32a940-164f-4bb1-b1a2-91048d6429eb/2808c91937524827a36d63eb5dbba702/deep/0/form-input-with-button.png)

1. Input field with label

	![](https://www.evernote.com/shard/s38/sh/b786250e-9fb0-4cf1-b8e8-b6af6ca416d0/abb43706f9716b7b67e32d26f67b9f27/deep/0/form-input-with-label.png) -->

####Dropdown
1. Dropdown normal

	![](https://www.evernote.com/shard/s38/sh/41f48b2d-be53-49e4-9ccf-b61d89aecc5a/8b94585c96965b9aa3405d35b8bbea25/deep/0/form-dropdown-normal.png)

	HTML:

	```html
	<select name="Dropdown">
		<option value="option1">Option 1</option>
		<option value="option2">Option 2</option>
		<option value="option3">Option 3</option>
	</select>
	```

	CSS:

	```css
	select {
		-webkit-appearance: button;
		background-image: url('img/icon-arrow-down.png'), linear-gradient(-180deg, #FFFFFF 0%, #F8F8F8 100%);
		background-position: 95% center;
		background-repeat: no-repeat;
		width: 300px;
		padding: 8px 14px;
		margin-bottom: 10px;
		border: 1px solid #DADADA;
		border-radius: 2px;	
		color: #999999;
		font-size: 14px;
		text-overflow: ellipsis;
		overflow: hidden;
		white-space: nowrap;
	}
	select:hover {
		cursor: pointer;
	}
	```

<!--1. Dropdown active

	![](https://www.evernote.com/shard/s38/sh/acf62bb4-e84a-46e7-9977-e0b279854034/7a3ca9e019efe0f2390a9e01c97b2a82/deep/0/form-dropdown-normal-active.png)-->


##Buttons and Switches<a name="#buttons-switches"></a>
####Regular buttons

This is the base code for all regular buttons. To use it, pair it with one styling class like `.btn-primary`.

HTML:

```html
<button type="button" class="btn-regular btn-primary"></button>
```

CSS:

```css
.btn-regular {
	padding: 8px 14px;
	margin: 5px;
	border-radius: 3px;
	font-size: 14px;
	cursor: pointer;
}
```

1. Regular primary button

	![](https://www.evernote.com/shard/s38/sh/edad2bae-7724-4bb8-805d-eab7b4536b49/438ebc2234d57cf3b45d61983a6e3088/deep/0/btn-regular-primary.png)

	HTML:

	```html
	<button type="button" class="btn-regular btn-primary"></button>
	```

	CSS:

	```css
	.btn-primary {
		background-image: linear-gradient(-180deg, #3F93F2 0%, #1574E1 100%);
		border: 1px solid #0E63C4;
		color: #FFFFFF;
	}
	.btn-primary:hover {
		background-image: linear-gradient(0deg, #2484F3 0%, #1780D5 100%);
	}
	```

1. Regular danger button

	![](https://www.evernote.com/shard/s38/sh/8a330ef5-89d4-4ab2-a4e5-67e0d36013e4/46b695c95e4401a5d443ad2b08212698/deep/0/btn-regular-danger.png)

	HTML:

	```html
	<button type="button" class="btn-regular btn-danger"></button>
	```

	CSS:

	```css
	.btn-danger {
		background-image: linear-gradient(-180deg, #EB2A2A 0%, #CE2929 100%);
		border: 1px solid #C70D24;
		color: #FFFFFF;
	}
	.btn-danger:hover {
		background-image: linear-gradient(0deg, #D91D1D 0%, #CE2824 100%);
	}
	```

1. Regular normal button

	![](https://www.evernote.com/shard/s38/sh/e3b19b7f-08a5-40fb-bfa5-e82e5673b34a/331fbdc48c66233cd3a755f916168261/deep/0/btn-regular-default.png)

	HTML:

	```html
	<button type="button" class="btn-regular btn-normal"></button>
	```

	CSS:

	```css
	.btn-normal {
		background-image: linear-gradient(-180deg, #FFFFFF 0%, #F8F8F8 100%);
		border: 1px solid #DADADA;
		color: #999999;
	}
	.btn-normal:hover {
		background-image: linear-gradient(0deg, #FAFAFA 0%, #F0F0F0 100%);
	}
	```

<!--1. Regular default button with options

	![](https://www.evernote.com/shard/s38/sh/4306c166-e644-4fd3-b873-cbe6e2ea2c08/293828b6efb3c6ffca801e9a99baaa2b/deep/0/btn-regular-default-options.png)-->

1. Regular disabled button

	![](https://www.evernote.com/shard/s38/sh/1b8f2480-7e35-40ef-b881-b2503a6af4c1/5b694d058e12f7778f0e924fa3ed448a/deep/0/btn-regular-disabled.png)

	HTML:

	```html
	<button type="button" class="btn-regular" disabled></button>
	```

	CSS:

	```css
	.btn-regular:disabled, .btn-small:disabled {
		background: #EEEEEE;
		color: #999999;
		cursor: default !important;
	}
	```

1. Regular button group

	![](https://www.evernote.com/shard/s38/sh/84e0d356-3c63-44cd-94ab-bb0860efa239/914934d74f0312644b0a7c6484cbc766/deep/0/btn-regular-group.png)

	HTML:

	```html
	<div class="btn-group">
		<button type="button" class="btn-regular btn-normal"></button>
		<button type="button" class="btn-regular btn-normal"></button>
		<button type="button" class="btn-regular btn-normal"></button>
	</div>
	```

	CSS:

	```css
	.btn-group {
		display: inline-block;
	}
	.btn-group button {
		float: left;
	  margin: 0;
	  margin-left: -3px;
	}
	.btn-group button:first-child {
		border-top-right-radius: 0;
		border-bottom-right-radius: 0;
	}
	.btn-group button:last-child {
		border-top-left-radius: 0;
		border-bottom-left-radius: 0;
	}
	.btn-group button:not(:first-child):not(:last-child) {
		-webkit-border-radius: 0;
		        border-radius: 0;
	}
	```

####Small buttons

Small buttons use the same styling classes as the regular buttons. The only difference is the use of the preceding class `.btn-small` instead of `.btn-regular`.

HTML:

```html
<button type="button" class="btn-small
 btn-primary"></button>
```

CSS: 

```css
.btn-small {
	padding: 4px 8px;
	margin: 3px;
	border-radius: 2px;
	font-size: 12px;
	cursor: pointer;
}
```

1. Small primary button

	![](https://www.evernote.com/shard/s38/sh/0b19c9ff-a95e-487b-9941-b19d54c3edf8/158da3b62730f1996adad00aa8eab445/deep/0/btn-small-action.png)

1. Small default button

	![](https://www.evernote.com/shard/s38/sh/d796661d-6f3f-46ad-8e02-3d309a54ab2a/b6da7e5cba598e3b4dc1d8fd8ec0655d/deep/0/btn-small-default.png)

1. Small disabled button

	![](https://www.evernote.com/shard/s38/sh/9a49a271-decf-40d0-8600-9555d04daed7/5fa843f48a313237ece7aced6005d79b/deep/0/btn-small-disabled.png)

1. Small button group

	![](https://www.evernote.com/shard/s38/sh/7579a13a-6143-4051-8af6-72ef635fcc40/c6e45be2685586983905232e43c4dd59/deep/0/btn-small-group.png)

####Switches
1. Switch (On)

	![](https://www.evernote.com/shard/s38/sh/4ac61084-ed97-44b9-bfe2-cfc637f1234a/5f3bfd52d271bfe2f6672f6f0e2a0df3/deep/0/btn-switch-yes.png)

1. Switch (Off)

	![](https://www.evernote.com/shard/s38/sh/cc3b132f-8b33-4951-82bb-896201ee0626/8a2ed1211eedba99c0f3aae1c402c970/deep/0/btn-switch-no.png)

####Checkboxes/Radio
1. Checkbox

	![](https://www.evernote.com/shard/s38/sh/fa67bc3a-a138-4d10-a731-b5f8c1082c05/237f7cbdd64ea3f06c1d8150fa2f7ff1/deep/0/btn-checkbox.png)

1. Radio

	![](https://www.evernote.com/shard/s38/sh/16cea9bf-5d7a-4a9d-99ce-227613b325d7/f686b947fb8b67906bbe65c708afac21/deep/0/btn-radio.png)

##Tables<a name="#tables"></a>
1. Table (Basic)

	![](https://www.evernote.com/shard/s38/sh/31f96424-cc68-4858-9782-3c19b3595089/3904a33e02a38bb31f899547cbdaa4ae/deep/0/table-basic.png)

1. Table (With controls)

	![](https://www.evernote.com/shard/s38/sh/d6407ed9-caed-4fc9-822d-b62005846d0e/b4edf17c4fe158954a8129c9c67c8567/deep/0/table-with-controls.png)

##Alerts<a name="#alerts"></a>
####Basic alerts
1. Info

	![](https://www.evernote.com/shard/s38/sh/84f49328-2aaf-42a3-b1eb-d769fdc84e45/263655dd0014efb037e50c2a66d1cbef/deep/0/alert-basic-info.png)

1. Success

	![](https://www.evernote.com/shard/s38/sh/1d9af14a-4f9b-43be-91a3-ed6e3149a006/053f86b1485c7174e9069bf95edf71a9/deep/0/alert-basic-success.png)

1. Error

	![](https://www.evernote.com/shard/s38/sh/3d428f08-effe-4eff-b1b2-621ff80df43b/60ac2e90acd0812ac1db9789686f0050/deep/0/alert-basic-error.png)

1. Danger

	![](https://www.evernote.com/shard/s38/sh/3c7cc9f1-4ac8-4414-9d00-8e44baf0f3e6/52e821e8bbb7c324326ea568837bc347/deep/0/alert-basic-danger.png)


####Feedback alerts
1. Info

	![](https://www.evernote.com/shard/s38/sh/274be7d9-5961-44d3-86ea-bf89f9f51b61/19b0f647164787623413f818a6374a7c/deep/0/alert-feedback-info.png)
	
1. Success

	![](https://www.evernote.com/shard/s38/sh/0aeb72ed-3318-4a8f-a0ef-87bab7ffe458/0d8ba3fef2e10bea11979652081e6ab7/deep/0/alert-feedback-success.png)
	
1. Error

	![](https://www.evernote.com/shard/s38/sh/2ea07da6-cda2-4ee8-9504-07ffc2e20a5d/9cef08193155cfe0c5763f108cb60455/deep/0/alert-feedback-warning.png)
	
1. Danger

	![](https://www.evernote.com/shard/s38/sh/93d39c7c-1a3f-4d02-a387-0b29ae9a9c81/bc804f8fa918010b0d69f4e0f116e1a8/deep/0/alert-feedback-danger.png)

##Dialogs<a name="#dialogs"></a>
1. Big modal

	![](https://www.evernote.com/shard/s38/sh/09c9f4f2-0697-4766-8095-979a83808cd1/fce2236e883765b355d41b5e46c194d5/deep/0/modal-big.png)

1. Small modal

	![](https://www.evernote.com/shard/s38/sh/9c578bee-5ab8-4cfe-a7d1-dadf2112a242/b0b893b67b71fae88a562c110f10d40e/deep/0/modal-small.png)
