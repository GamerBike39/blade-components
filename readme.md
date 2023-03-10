# Blade Components

### User's Guide

After the prerequisites that require you to have Laravel, Blade and Tailwinds installed.

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
                                           {{ $quiz->title }}
                                        </x-slot>
                                        <x-slot name="itemId">
                                            {{ $quiz->id }}
                                        </x-slot>
                                    </x-confirm-delete>