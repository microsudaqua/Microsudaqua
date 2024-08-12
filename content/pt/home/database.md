+++
# Any elements can be added in the body: https://sourcethemes.com/academic/docs/writing-markdown-latex/
# Add more sections by duplicating this file and customizing to your requirements.

widget = "blank"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 0 # Order that this section will appear.


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

 
{{% staticref "files/Metz-Huber_et_al-2022-a georeferenced rRNA amplicon database of aquatic microbiomes from South America.pdf" "newtab" %}}**µSudAqua[db]: Uma base de dados georreferenciada de rRNA amplicon de microbiomas aquáticos da América do Sul‌**{{% /staticref %}}

*A biogeografia de comunidades bacterianas é um tópico-chave na Ecologia Microbiana. Em relação à águas continentais, muitos estudos foram realizados no hemisfério norte, deixando uma lacuna nos padrões de diversidade microbiana em uma escala global. A América do Sul abriga cerca de um terço de toda a água doce do mundo, mas é uma das regiões menos estudadas. Para preenxer esta lacuna, nós compilamos dados de sequenciamento amplicom do gene 16S rRNA de comunidades microbianas abarcando os ecossistemas de águas continentais sulamericanos, e apresentamos a primeira base de dados µSudAqua[db]. Esta base de dados contém mais de 872 amostras georreferenciadas de 9 diferentes ecoregiões contendo informações ambientais para cada uma delas. Para sua integração e validação, nós construímos uma base de dados curada (µSudAqua[db.sp]) de amostras sequenciadas na plataforma Illumina MiSeq e os mesmos primers universais para procariotos. Isto compõe cerca de 60% de todas as amostras georreferenciadas contidas na µSudAqua[db]. Esta compilação foi realizada na escopo da rede colaborativa µSudAqua e representa uma das mais completas bases de dados de comunidade microbianas de águas continentais da América do Sul.* Veja a [documentação](https://github.com/microsudaqua/usudaquadb) para mais detalhes, ou acesse a [base de dados](https://doi.org/10.5281/zenodo.6802178).