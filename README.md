## HTML formatter class.

A simple to use HTML prettifier class written in PHP.

### Example:

    <?php
    include_once('format.php');

    $html = 'Unformatted HTML string';

    // initialize class
    $format = new Format();

    // use spaces at 4 length
    echo $format->html($html);

    // use spaces at 2 length
    echo $format->html('Unformatted HTML string', true, 2);

    // use tabs
    echo $format->html('Unformatted HTML string', false);

### Static method example:

    <?php
    include_once('format.php');

    $html = 'Unformatted HTML string';

    // use spaces at 4 length
    echo Format::HTML($html);

    // use spaces at 2 length
    echo Format::HTML($html, true, 2);

    // use tabs
    echo Format::HTML($html, false);
