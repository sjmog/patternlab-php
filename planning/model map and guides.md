settings
	logo_url

image
	url
	alt

video
	versions: 
		mp4, 
		webm, 
		ogg
	url
	name
	-> poster (carrierwave)

audio
	url




Notes

logo.png is the logo.
ajax-loader.gif is the ajax loading symbol.
favicons are favicon-32x32.jpg and favicon-16x16.jpg and they are stored in the assets folder.




Build Notes

Patterns are partials ONLY IF included in an iterator, with model name substitution as follows:

@videos.each do |video|
	<%= render partial: '00-atoms/08-media/00-video', locals: {video: video} %>
end