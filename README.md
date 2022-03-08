# 
<html lang="ar-rMY">
<head>
	<meta charset="UTF-8">
	<title>Animasi Ikan di Aquarium</title>
	<link rel="stylesheet" href="style.css">
  <style>
  body{
	margin:0;
	padding:0;
	background: yellow;
}

.aqua{
	position: absolute;
	top:50%;
	left:50%;
	transform: translate(-50%, -50%);
	width: 300px;
	height: 300px;
	background: rgba(255,255,255,0.1);
	border-radius: 50%;
	border:4px solid black;
	transform-origin: bottom center;
	animation: animate 5s linear infinite;
}

.aqua:before
{
	content:'';
	position: absolute;
	top:10px;
	left:8%; 
	transform: rotate(-27deg) ; 
	width: 40%;
	height:30px;
	background: rgba(113, 107, 107, 0.61);
	border:4px solid #ffffff;
	border-radius: 50%;
}

.aqua:after
{
	content:'';
	position: absolute;
	top: 17%;
	left: 20%;
	transform: rotate(-25deg);
	width: 100px;
	height: 30px;
	background: rgba(255,255,255,0.05);
	border-radius: 50%;
}

.air{
	position: absolute;
	top:50%;
	left:5px;
	right: 5px;
	bottom:5px;
	background: rgba(65,193,251,0.5);
	border-bottom-right-radius: 150px;	
	border-bottom-left-radius: 150px;
	transform-origin: top center;	
	animation: animateair 5s linear infinite;
}

.air:before{
	content:'';
	position: absolute;
	top:-10px;
	left:0;
	width: 100%;
	height: 20px;	
	background: rgba(75, 203, 224, 0.97);
	border-radius: 50%;
}

.shadow
{
	position: absolute;
	top:calc(50% + 150px);
	left:50%;
  transform:translate(-50%, -50%);
  width: 250px;
  	height: 30px;
  background:rgba(150, 141, 141, 0.2);
	z-index: -1;
	border-radius: 50%;
}

img.iwak
{
	width: 25px;
  height: 75px;
	animation: animateIwak 10s linear infinite;
}
  img.iemas
  {
    width: 75px;
    height: 75px;
    animation: animateIemas 10s linear infinite;
  }

/* digunakan untuk animasi ikan bergerak*/

@keyframes animateIemas
{
	0%
	{
		transform: translate(0,0) rotateY(180deg);
	}
	50%
	{
		transform: translate(190px,0px) rotateY(180deg);
	}
	51%
	{
		transform: translate(200px,0px) rotateY(0deg);
	}
	100%
	{
		transform: translate(0,0) rotateY(0deg);
	}
}

/* digunakan untuk animasi dari aquarium */

@keyframes animate
{
	0%
	{
		transform: translate(-50%, -50%) rotate(0deg);
	}
	25%
	{
		transform: translate(-50%, -50%) rotate(15deg);
	}
	50%
	{
		transform: translate(-50%, -50%) rotate(0deg);
	}
	75%
	{
		transform: translate(-50%, -50%) rotate(-15deg);
	}
	100%
	{
		transform: translate(-50%, -50%) rotate(0deg);
	}
}

/*digunakan untuk animasi air*/

@keyframes animateair 
{
	0%
	{
		transform: rotate(0deg);
	}
  25%
	{
		transform: rotate(-20deg);
	}
	50%
	{
		transform: rotate(0deg);
	}
	75%
	{
		transform: rotate(20deg);
	}
	100%
	{
		transform: rotate(0deg);
	}
}
  </style>
  <script type="text/javascript">
window.location = "https://budaksixteen16.github.io/Jadual-lengkap-jawi";
</script>

</head>
<body>
	<div class="aqua">
		<div class="air">	
			<img src="https://blogger.googleusercontent.com/img/a/AVvXsEhky7rFI8mpz2vsyYdJFUTtx6ZFX4KNRRmBR598zQqFx_6wz8g7T3KfwcL4PB2qRQGjHxKoHFlHgp2vwUgspoLPkoxVEDvIp93WZEUgHCSzxlUhlQzAPv_kzKYi3sXnpptRKFMPVKy9jhP-U4oyBxnxa5duUCev2-MTIuFoh2Al1CTOW0M4b8PqT-MG=s525" class="iwak" alt="iwak">		
		  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEiBmdrt39jwN_n4RMJN-x0xn6s1_Nf2cuUpp6iEIKusOh5svxxsGW6dMRdb12YNkJm_LX8I_vwO0sQcniN6bEu4sYS4oaaSQnRkT_x6QLX75zbxPvnPinagzSL8l8LE-3aejeNV42TiFIe1CAfPUCYHr6jpxqPrC-7FxOf-hdzIXM0jpdHWmgNU9ENA=s790" class="iemas" alt="iemas">
		  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEiZ_yaBqm2cdv2D2dVBv5tSo-lFqewICfuwCgLE_qKwcPnKE9kJKPUkIkjGeLn2KMS--XR6la3iZi5AXfMImLBcfXK1C9XR4uLyLFAXxPak5MWb9SpbHpZBFbU0shRq2I64n0Yhzm-qqgGEcwSfn2YM2-a1zcsPXA1EJcIZFQSsn8GMJSF6TYNat_JT=s960" class="iemas" alt="iemas">
		  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEgAms_4jYC8in7vIE8c2fqE_d_fQrukedpPjEWfLF-WVI_3o9UI5aV7OaFvao_SKc4CAtOPyf477n7txPkRVT6QziE7vQLGHe_2uq6UpJFQgqHlwgemabk_LITPT-zlvSVdIlnArBJB4i3pCzUDSjLCx_sX4ZDlGQjasd1P7ABogP2KLpWDcDHCrQcG=s500" class="iemas" alt="iemas">
		</div>
	</div>
	<div class="shadow"></div>
	<div dir="rtl" class="Font">ممواتكن...</div><div dir="rtl" class="Font">Loading...</div>
</body>
	<style>
@import url('https://fonts.googleapis.com/css2?family=Amiri&display=swap');

.Font {
  font-family: 'Amiri', serif;
</style>
</html>
