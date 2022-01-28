+++
# Any elements can be added in the body: https://sourcethemes.com/academic/docs/writing-markdown-latex/
# Add more sections by duplicating this file and customizing to your requirements.

widget = "blank"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 120 # Order that this section will appear.


title = "Database"
# subtitle = "Red Colaborativa en ecologia Microbiana de América Latina"

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "1"

[design.background]
  # Apply a background color, gradient, or image.
  #   Uncomment (by removing `#`) an option to apply it.
  #   Choose a light or dark text color by setting `text_color_light`.
  #   Any HTML color name or Hex value is valid.

  # Background color.
   color = "Grey10"
  
  # Background gradient.
  #gradient_start = "DarkBlue"
  #gradient_end = "Cyan"
  
  # Background image.
  # image = "image.jpg"  # Name of image in `static/img/`.
  # image_darken = 0.6  # Darken the image? Range 0-1 where 0 is transparent and 1 is opaque.
  # image_size = "cover"  #  Options are `cover` (default), `contain`, or `actual` size.
  # image_position = "center"  # Options include `left`, `center` (default), or `right`.
  # image_parallax = true  # Use a fun parallax-like fixed background effect? true/false
  
  # Text color (true=light or false=dark).
  text_color_light = false

[design.spacing]
  # Customize the section spacing. Order is top, right, bottom, left.
  padding = ["20px", "0", "20px", "0"]

[advanced]
 # Custom CSS. 
 css_style = ""
 
 # CSS class.
 css_class = ""
+++
**µSudAqua[db]: a georeferenced rRNA amplicon database of aquatic microbiomes from South America‌**
 
{{% staticref "files/libro_2019.pdf" "newtab" %}}inprep article{{% /staticref %}}

*The biogeography of bacterial communities is a key topic in Microbial Ecology. Regarding continental water, most studies are carried out in the northern hemisphere, leaving a gap on microorganism’s diversity patterns on a global scale. South America harbours approximatelly one third of the world's total fresh water resources, and is one of these understudied regions. To fill this gap, we compiled 16S rRNA amplicon sequencing data of microbial communities across South America continental water ecosystems, presenting the first database µSudAqua[db]. The database contains over 872 georeferenced samples from 9 different ecoregions with contextual environmental information. For its integration and validation we constructed a curated database (µSudAqua[db.sp]) using samples sequenced in Illumina MiSeq platform using the same prokaryote universal primers. This comprised ~60% of the total georeferenced samples of the µSudAqua[db]. This compilation was carried out in the scope of the µSudAqua collaborative network and represents one of the most complete databases of continental water microbial communities from South America.* See the [documentation](https://github.com/microsudaqua/usudaquadb) for more details, or access the [database](http://200.9.237.240:9005/usudaqua/).