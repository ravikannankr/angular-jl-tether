ng-tether
=========

[Tether](http://tether.io) wrapper for Angular, so you can use it in directives declaratively. **Tether is included**

Not to be mistaken for a very cool project called [`angular-tether`](https://github.com/nissoh/angular-tether) that is in the process of implementing Tether in angular.

# Install

`bower install ng-tether` or `npm install ng-tether`

# Usage

```html
<div ng-tether ng-tether-options="{
    target: '.target',
    attachment: 'top left',
    targetAttachment: 'top right'
}"></div>
```

or

```html
<div ng-tether 
 ng-tether-target=".target" 
 ng-tether-attachment="top left"
 ng-tether-target-attachment="top right"></div>
```

You can grab a reference to the Tether object if you want by passing a string into `ng-tether`. 

```html
<div ng-tether="ngTetherReference" 
 ng-tether-target=".target" 
 ng-tether-attachment="top left"
 ng-tether-target-attachment="top right"></div>
```

`ngTetherReference` will now be in `$scope`. You can do things like

```html
<div ng-click="ngTetherReference.destroy()">kind of a button</div>
```

To destroy it. 

You can see the [Tether docs](http://tether.io) for a full list of options and api functions. 


# Building

`npm run deps` to get the dependencies  
`npm run dist` to build  
`npm run watch` to continuously build   

I've never been to the Empire State building
