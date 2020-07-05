## Install
You can install this package via composer.
```
composer require bijay/array2xml
```

## Usage

```
include 'vendor/autoload.php'
use Bijay\Array2Xml\Array2Xml;

$array = [
    'First node' => [
        'name' => 'Bijaya Oli',
        'address' => 'Bhaktapur'
    ],
    'Second node' => [
        'name' => 'Ugyen Chheda Lama',
        'address' => 'Kathmandu'
    ]
];
```
```
$result = Array2Xml::convert($array);
```
## After running this piece of code $result will contain:
```
<?xml version="1.0"?>
<root>
    <First_node>
        <name>Bijaya Oli</name>
        <weapon>Bhaktapur</weapon>
    </First_node>
    <Second_node>
        <name>Ugyen Chheda</name>
        <weapon>Kathmandu</weapon>
    </Second_node>
</root>
```
