# Kohana-HTML2PDF convert #
  
* Module Versions: 1.1 *
* Module URL: https://github.com/abaranovskiy/Kohana-html2pdf
* Origin Module URL: https://github.com/sudeste/Kohana-html2pdf
* Compatible Kohana Version(s): 3.3.x

-----------------------------------------------------------
## Description ##
 Module Kohana for convert HTML to PDF using class HTML2PDF


-----------------------------------------------------------
## Requirements & Installation ##

1. install module in bootstrap.php

3. In config file sets Your locate 


-----------------------------------------------------------
## Using ##

* In Controller

1.
Set up a configuration data

<pre>
<code>

       $config = array(
                'author'   => 'Your name',
                'title'    => 'Your title',
                'subject'  => 'Your subject',
                'name'     => Text::random().'.pdf', // name file pdf
        );
</code>
</pre>

2.
Geterate an pdf from HTML

<pre>
<code>
$view = View_PDF::factory('admin/report/pdf', $config)
        ->set('variable', $Data)
        ->render();
</code>
</pre>


