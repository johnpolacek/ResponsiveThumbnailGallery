#jQuery Responsive Thumbnail Gallery

jQuery Plugin for creating image galleries that scale to fit their container.

##How to Use

Link to the script after jQuery. Apply it to a DOM element on the document ready event.

	$(document).ready(function() {
		var gallery = new $.ThumbnailGallery($('#gallery'));
	});
    
You can configure the settings as follows (example has the default config values assigned):

	$(document).ready(function() {
		var gallery = new $.ThumbnailGallery($('#gallery'), {
            thumbImages: '_/img/thumbs/thumb',
            smallImages: '_/img/small/image',
            largeImages: '_/img/large/image',
            count: 10,
            thumbImageType: 'jpg',
            imageType: 'jpg',
            breakpoint: 600,
            shadowStrength: 1
        });
	});
    

Parameters are:
    
**thumbImages:** path to the thumbnails  
**smallImages:** path to the small size images  
**largeImages:** path to the large size images  
**count:** number of images/thumbnails  
**thumbImageType:** file extension for thumbnail images (all should be the same)  
**imageType:** file extension for gallery images (all should be the same)  
**breakpoint:** width at which the small and large image sizes are swapped  
**shadowStrength:** strength of the shadow on the non-selected thumbs (0-1)  


jQuery Responsive Thumbnail Gallery Plugin created by John Polacek  
Twitter: http://twitter.com/#!/johnpolacek  
Blog: http://johnpolacek.com

