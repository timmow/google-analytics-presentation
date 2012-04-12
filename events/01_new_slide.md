!SLIDE bullets
# Events #
 * Capture interactions that are not pageviews
 * Does not add a pageview
 * Can capture more than just user interactions
!SLIDE bullets
# Examples #
 * Ajax galleries
 * 404 tracking
 * Search 0 results
!SLIDE  bullets

# Tracking code example #
	@@@ javascript
	_gaq.push(['_trackEvent',
	 'Category', 'Action', 
	 'Label', 'Value', 'noninteraction']);

 * Category, action, label, value as seen in reports
 * noninteraction boolean paramater affects bounce rate

!SLIDE 
# jQuery event
	@@@ javascript
	<a id="button">button</a>

	$('button').
	click(
	function() {
	// do something fun
	_gaq.push(['_trackEvent',
	 'Buttons', 'Clicked']) 
	});




