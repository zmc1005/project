<!DOCTYPE html>
<html>
<head>
<script type="text/javascript" src="cordova.js"></script>
<link rel="stylesheet" href="http://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.css" />
<script type="text/javascript" src="http://code.jquery.com/jquery-1.11.1.min.js"></script>
<script type="text/javasript">
		$(function() {
			function camPic(imgData) {
			$("img_cam").attr("src", imgData)
			}
			
			function camFail() {
			alert(fail);
			}
			
			function camAccess {
				var options = {
					destinationType: Camera.DestinationType.FILE_URI,
					sourceType: Camera.PictureSourceType.CAMERA
				
				};
				navigator.camera.getImg(camPic, camFail, options);
			}
			$(#camera_btn).on("click", camAccess);
		});


</script>

<script type="text/javascript"  src="http://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.js"></script>
<meta charset="utf-8">
</head>
<body>
	<div data-role="page">
		<div data-role="page">
		<h1>Homework Camera App</h1>
		</div>
			<div class="ui-content">
			<button id="camera_btn">Camera</button>
			<img id="img_cam">
	</div>


</body>
</html>
