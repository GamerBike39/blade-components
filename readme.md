# Blade Components

### User's Guide

you will need the TALL stack

You have to put the files in the components folder.
This folder is located in: 
resources -> views -> components

For example for confirm-delete.blade.php
you can see that the file starts with
```sh
@props(['subject', 'itemId'])
```


This represents the variables of the component.
To use these components in your views, you will need to use the following directive:

```sh
<x-confirm-delete>

  <x-slot name='subject'>
     {{ **** }}
  </x-slot>
  
  <x-slot name="itemId">
     {{ $***->id }}
   </x-slot>
   
</x-confirm-delete>
