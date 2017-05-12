# opencart-array-helper

Opencart Array Helper provides additional array functionality that you can use in your application.

For more details and usage information on ArrayHelper, see the [guide article on array helpers](http://www.yiiframework.com/doc-2.0/guide-helper-array.html).
###
This module from Yii2 Framework is adapted by [Mefistophell Nill](https://github.com/Mefistophell) and [Zoturn](https://github.com/Zoturn) (**8sun Empire**) especially for OpenCart.

Tested on Opencart 2.0. If you find an error, let us know.

Version: 1.0

See also: [Opencart Html Helper](https://github.com/8sun/opencart-html-helper)

## Install
1. You need copy the files to `/system/helper/` directory.

2. Further add Helpers to `/system/startup.php` how is shown below:

```
require_once(DIR_SYSTEM . 'helper/ArrayHelper.php');
require_once(DIR_SYSTEM . 'helper/InvalidParamException.php');
```

## Usage
Just use Helpers into your template files. You may get something following:

```
$array = [
    ['id' => '123', 'data' => 'abc'],
    ['id' => '345', 'data' => 'def'],
];
$result = ArrayHelper::getColumn($array, 'id');
// the result is: ['123', '345']
```

Here is the list of available features

<table>
    <colgroup>
        <col class="col-method">
        <col class="col-description">
    </colgroup>
    <tbody>
        <tr>
            <th>Method</th><th>Description</th>
        </tr>
        <tr id="filter()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#filter()-detail">filter()</a></td>
            <td>Filters array according to rules specified.</td>
        </tr>
        <tr id="getColumn()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#getColumn()-detail">getColumn()</a></td>
            <td>Returns the values of a specified column in an array.</td>
        </tr>
        <tr id="getValue()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#getValue()-detail">getValue()</a></td>
            <td>Retrieves the value of an array element or object property with the given key or property name.</td>
        </tr>
        <tr id="htmlDecode()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#htmlDecode()-detail">htmlDecode()</a></td>
            <td>Decodes HTML entities into the corresponding characters in an array of strings.</td>
        </tr>
        <tr id="htmlEncode()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#htmlEncode()-detail">htmlEncode()</a></td>
            <td>Encodes special characters in an array of strings into HTML entities.</td>
        </tr>
        <tr id="index()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#index()-detail">index()</a></td>
            <td>Indexes and/or groups the array according to a specified key.</td>
        </tr>
        <tr id="isAssociative()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#isAssociative()-detail">isAssociative()</a></td>
            <td>Returns a value indicating whether the given array is an associative array.</td>
        </tr>
        <tr id="isIn()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#isIn()-detail">isIn()</a></td>
            <td>Check whether an array or <a href="http://www.yiiframework.com/doc-2.0/http://www.php.net/class.traversable">Traversable</a> contains an element.</td>
        </tr>
        <tr id="isIndexed()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#isIndexed()-detail">isIndexed()</a></td>
            <td>Returns a value indicating whether the given array is an indexed array.</td>
        </tr>
        <tr id="isSubset()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#isSubset()-detail">isSubset()</a></td>
            <td>Checks whether an array or <a href="http://www.yiiframework.com/doc-2.0/http://www.php.net/class.traversable">Traversable</a> is a subset of another array or <a href="http://www.yiiframework.com/doc-2.0/http://www.php.net/class.traversable">Traversable</a>.</td>
        </tr>
        <tr id="isTraversable()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#isTraversable()-detail">isTraversable()</a></td>
            <td>Checks whether a variable is an array or <a href="http://www.yiiframework.com/doc-2.0/http://www.php.net/class.traversable">Traversable</a>.</td>
        </tr>
        <tr id="keyExists()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#keyExists()-detail">keyExists()</a></td>
            <td>Checks if the given array contains the specified key.</td>
        </tr>
        <tr id="map()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#map()-detail">map()</a></td>
            <td>Builds a map (key-value pairs) from a multidimensional array or an array of objects.</td>
        </tr>
        <tr id="merge()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#merge()-detail">merge()</a></td>
            <td>Merges two or more arrays into one recursively.</td>
        </tr>
        <tr id="multisort()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#multisort()-detail">multisort()</a></td>
            <td>Sorts an array of objects or arrays (with the same structure) by one or several keys.</td>
        </tr>
        <tr id="remove()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#remove()-detail">remove()</a></td>
            <td>Removes an item from an array and returns the value. If the key does not exist in the array, the default value
                will be returned instead.</td>
        </tr>
        <tr id="removeValue()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#removeValue()-detail">removeValue()</a></td>
            <td>Removes items with matching values from the array and returns the removed items.</td>
        </tr>
        <tr id="toArray()">
            <td><a href="http://www.yiiframework.com/doc-2.0/yii-helpers-basearrayhelper.html#toArray()-detail">toArray()</a></td>
            <td>Converts an object or an array of objects into an array.</td>
        </tr>
    </tbody>
</table>
