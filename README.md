# Pagina personal

Vista previa de la web 2017: [LINK](https://all4gis.github.io/)

![](sceenshot/captura.png?raw=true)


Los pasos para crear una sitio web de Github partiendo de cero y empleando un template como base son:

 - Los templates disponibles son:

	[Templates](https://github.com/jekyll/jekyll/wiki/Themes)

Nos descargamos el que más nos guste y empezamos,(**Tested in Windows 10**)
 

 - Instalamos Ruby y el pack DevKit

 [Ruby](https://rubyinstaller.org/downloads/)  

Nos dirigimos donde hemos instalado el paquete :

    devkit

    ruby dk.rb init

    ruby dk.rb install

 - Instalamos node.js

 [Node.js](https://nodejs.org/es/download/)

 - Instalamos Bundler desde consola:
 

		gem install bundler
    
 - Instalamos Jekyll desde consola:

		gem install jekyll

 - Vamos donde hemos instalado Jekyll y tecleamos:

		jekyll new myfirstsite
		cd myfirstsite
		jekyll serve

**Nota:**
Si da el fallo de `github-pages x64-mingw32` es por el DevKit de Ruby una vez lo tengamos ,por si no lo instalamos anteriormente,ponemos

    bundle install
    gem cleanup
	
 - Arrancamos el servidor local

		bundle exec jekyll serve --config _config.yml

Vamos a `http://localhost:4000/`  para ver la web

Template empleado en esta web como base : [Template](https://github.com/sergiokopplin/indigo)

[© All4gis 2017]
