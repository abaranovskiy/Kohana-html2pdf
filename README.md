# Kohana-HTML2PDF convert #
  
* Module Versions: 1.0 *
* Module URL: https://github.com/sudeste/Kohana-html2pdf
* Compatible Kohana Version(s): 3.2.x

-----------------------------------------------------------
## Description ##
 Module Kohana for convert HTML to PDF using class HTML2PDF


-----------------------------------------------------------
## Requirements & Installation ##

1. install module in bootstrap.php

2. Download class HTML2PDF http://www.html2pdf.fr/en/download e discharges in /vendor/html2pdf/

3. In config file sets Your locate 


-----------------------------------------------------------
## Using ##

* In Controller
Iniciando a configuração

'        $config = array(
                'author'   => 'Your name',
                'title'    => 'Your title',
                'subject'  => 'Your subject',
                'name'     => Text::random().'.pdf', // name file pdf
        );
'
Gerando o Html e exporting PDF
'
$view = View_PDF::factory('admin/report/pdf', $config)
        ->set('dados', $dados)
        ->render();
'

[!] View folder /example/ containing 

1. php file example code html.
2. example pdf generated.