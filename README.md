# Factorial.io components: Breadcrumb

A Factorial.io component to display a breadcrumb with configurable space and seperator.

## Configurable variables

* `--Breadcrumb-display`: defines the `display`-property of the items
* `--Breadcrumb-display-sm`: if `undefined` inherits the `--Breadcrumb-display` value
* `--Breadcrumb-display-md`: if `undefined` inherits the `--Breadcrumb-display-sm` value 
* `--Breadcrumb-display-lg`: if `undefined` inherits the `--Breadcrumb-display-md` value 
* `--Breadcrumb-spacing`: the spacing between item and seperator
* `--Breadcrumb-seperator`: the seperator between items
* `--Breadcrumb-link-color`: the link-color
* `--Breadcrumb-link-color-hover`: if `undefined` inherits the `--Breadcrumb-link-color` value
* `--Breadcrumb-link-color-visited`: if `undefined` inherits the `--Breadcrumb-link-color` value

## Configuration

The array the component needs looks like this:
```
$your_array = array(
  'breadcrumb' => array(
    array(
      'title' => 'Main Page',
      'url' => '/'
    ),
    array(
      'title' => 'Child Page',
      'url' => '/'
    ),
    array(
      'title' => 'Grandchild Page',
      'current' => 'true'
    ),
  )
)
```

## Usage

If you want to include the component in one of your template-files, just use

php
```php
  print component('factorial-io-components-breadcrumb', $your_array));
```
haml
```php
  = component('factorial-io-components-breadcrumb', $your_array)
```
 

