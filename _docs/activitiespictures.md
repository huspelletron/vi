---
title: Activities
permalink: /docs/activitiespictures/
---

<link href="https://www.jqueryscript.net/css/jquerysctipttop.css" rel="stylesheet" type="text/css">
<link href="https://www.jqueryscript.net/demo/Powerful-Multi-Functional-jQuery-Lightbox-Plugin-Magnific-Popup/dist/magnific-popup.css" rel="stylesheet" type="text/css">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
<script src="https://www.jqueryscript.net/demo/Powerful-Multi-Functional-jQuery-Lightbox-Plugin-Magnific-Popup/dist/jquery.magnific-popup.js"></script>
<style>
/* Basic Example */

.mfp-no-margins img.mfp-img {
padding: 0;
}
.mfp-no-margins .mfp-figure:after {
top: 0;
bottom: 0;
}
.mfp-no-margins .mfp-container {
padding: 0;
}
/**
 * Simple fade transition,
 */
.mfp-fade.mfp-bg {
opacity: 0;
-webkit-transition: all 0.15s ease-out;
-moz-transition: all 0.15s ease-out;
transition: all 0.15s ease-out;
}
.mfp-fade.mfp-bg.mfp-ready {
opacity: 0.8;
}
.mfp-fade.mfp-bg.mfp-removing {
opacity: 0;
}
.mfp-fade.mfp-wrap .mfp-content {
opacity: 0;
-webkit-transition: all 0.15s ease-out;
-moz-transition: all 0.15s ease-out;
transition: all 0.15s ease-out;
}
.mfp-fade.mfp-wrap.mfp-ready .mfp-content {
opacity: 1;
}
.mfp-fade.mfp-wrap.mfp-removing .mfp-content {
opacity: 0;
}
/* Styles for dialog window */
#small-dialog {
background: white;
padding: 20px 30px;
text-align: left;
max-width: 400px;
margin: 40px auto;
position: relative;
}
/**
 * Fade-zoom animation for first dialog
 */

/* start state */
.my-mfp-zoom-in #small-dialog {
opacity: 0;
-webkit-transition: all 0.2s ease-in-out;
-moz-transition: all 0.2s ease-in-out;
-o-transition: all 0.2s ease-in-out;
transition: all 0.2s ease-in-out;
-webkit-transform: scale(0.8);
-moz-transform: scale(0.8);
-ms-transform: scale(0.8);
-o-transform: scale(0.8);
transform: scale(0.8);
}
/* animate in */
.my-mfp-zoom-in.mfp-ready #small-dialog {
opacity: 1;
-webkit-transform: scale(1);
-moz-transform: scale(1);
-ms-transform: scale(1);
-o-transform: scale(1);
transform: scale(1);
}
/* animate out */
.my-mfp-zoom-in.mfp-removing #small-dialog {
-webkit-transform: scale(0.8);
-moz-transform: scale(0.8);
-ms-transform: scale(0.8);
-o-transform: scale(0.8);
transform: scale(0.8);
opacity: 0;
}
/* Dark overlay, start state */
.my-mfp-zoom-in.mfp-bg {
opacity: 0;
-webkit-transition: opacity 0.3s ease-out;
-moz-transition: opacity 0.3s ease-out;
-o-transition: opacity 0.3s ease-out;
transition: opacity 0.3s ease-out;
}
/* animate in */
.my-mfp-zoom-in.mfp-ready.mfp-bg {
opacity: 0.8;
}
/* animate out */
.my-mfp-zoom-in.mfp-removing.mfp-bg {
opacity: 0;
}
/**
 * Fade-move animation for second dialog
 */

/* at start */
.my-mfp-slide-bottom #small-dialog {
opacity: 0;
-webkit-transition: all 0.2s ease-out;
-moz-transition: all 0.2s ease-out;
-o-transition: all 0.2s ease-out;
transition: all 0.2s ease-out;
-webkit-transform: translateY(-20px) perspective( 600px ) rotateX( 10deg );
-moz-transform: translateY(-20px) perspective( 600px ) rotateX( 10deg );
-ms-transform: translateY(-20px) perspective( 600px ) rotateX( 10deg );
-o-transform: translateY(-20px) perspective( 600px ) rotateX( 10deg );
transform: translateY(-20px) perspective( 600px ) rotateX( 10deg );
}
/* animate in */
.my-mfp-slide-bottom.mfp-ready #small-dialog {
opacity: 1;
-webkit-transform: translateY(0) perspective( 600px ) rotateX( 0 );
-moz-transform: translateY(0) perspective( 600px ) rotateX( 0 );
-ms-transform: translateY(0) perspective( 600px ) rotateX( 0 );
-o-transform: translateY(0) perspective( 600px ) rotateX( 0 );
transform: translateY(0) perspective( 600px ) rotateX( 0 );
}
/* animate out */
.my-mfp-slide-bottom.mfp-removing #small-dialog {
opacity: 0;
-webkit-transform: translateY(-10px) perspective( 600px ) rotateX( 10deg );
-moz-transform: translateY(-10px) perspective( 600px ) rotateX( 10deg );
-ms-transform: translateY(-10px) perspective( 600px ) rotateX( 10deg );
-o-transform: translateY(-10px) perspective( 600px ) rotateX( 10deg );
transform: translateY(-10px) perspective( 600px ) rotateX( 10deg );
}
/* Dark overlay, start state */
.my-mfp-slide-bottom.mfp-bg {
opacity: 0;
-webkit-transition: opacity 0.3s ease-out;
-moz-transition: opacity 0.3s ease-out;
-o-transition: opacity 0.3s ease-out;
transition: opacity 0.3s ease-out;
}
/* animate in */
.my-mfp-slide-bottom.mfp-ready.mfp-bg {
opacity: 0.8;
}
/* animate out */
.my-mfp-slide-bottom.mfp-removing.mfp-bg {
opacity: 0;
}
</style>

<h2>Lightbox gallery</h2>
<div class="popup-gallery"> <a href="https://farm9.staticflickr.com/8242/8558295633_f34a55c1c6_b.jpg" title="The Cleaner"><img src="https://farm9.staticflickr.com/8242/8558295633_f34a55c1c6_s.jpg" width="75" height="75"></a> <a href="https://farm9.staticflickr.com/8382/8558295631_0f56c1284f_b.jpg" title="Winter Dance"><img src="https://farm9.staticflickr.com/8382/8558295631_0f56c1284f_s.jpg" width="75" height="75"></a> <a href="https://farm9.staticflickr.com/8225/8558295635_b1c5ce2794_b.jpg" title="The Uninvited Guest"><img src="https://farm9.staticflickr.com/8225/8558295635_b1c5ce2794_s.jpg" width="75" height="75"></a> <a href="https://farm9.staticflickr.com/8383/8563475581_df05e9906d_b.jpg" title="Oh no, not again!"><img src="https://farm9.staticflickr.com/8383/8563475581_df05e9906d_s.jpg" width="75" height="75"></a> <a href="https://farm9.staticflickr.com/8235/8559402846_8b7f82e05d_b.jpg" title="Swan Lake"><img src="https://farm9.staticflickr.com/8235/8559402846_8b7f82e05d_s.jpg" width="75" height="75"></a> <a href="https://farm9.staticflickr.com/8235/8558295467_e89e95e05a_b.jpg" title="The Shake"><img src="https://farm9.staticflickr.com/8235/8558295467_e89e95e05a_s.jpg" width="75" height="75"></a> <a href="https://farm9.staticflickr.com/8378/8559402848_9fcd90d20b_b.jpg" title="Who's that, mommy?"><img src="https://farm9.staticflickr.com/8378/8559402848_9fcd90d20b_s.jpg" width="75" height="75"></a> </div>
<script>
$(document).ready(function() {
	$('.popup-gallery').magnificPopup({
		delegate: 'a',
		type: 'image',
		tLoading: 'Loading image #%curr%...',
		mainClass: 'mfp-img-mobile',
		gallery: {
			enabled: true,
			navigateByImgClick: true,
			preload: [0,1] // Will preload 0 - before current, and 1 after the current image
		},
		image: {
			tError: '<a href="%url%">The image #%curr%</a> could not be loaded.',
			titleSrc: function(item) {
				return item.el.attr('title') + '<small>by Marsel Van Oosten</small>';
			}
		}
	});
});
</script>

<!-- {% include image-gallery.html folder="/uploads/activitiespictures" %} -->