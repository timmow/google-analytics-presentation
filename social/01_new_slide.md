!SLIDE bullets
# Social Tracking #
 * Similar to event tracking
 * Tailored towards events on social networks
 * Requires events fired by social networks
 * Facebook, Twitter, Google Plus all do
!SLIDE
# Examples #
!SLIDE smaller
# Facebook like #
	@@@ javascript
	FB.Event.subscribe('edge.create', 
	function(targetUrl) {
		_gaq.push(['_trackSocial',
		 'facebook', 'like', targetUrl]);
	});`

