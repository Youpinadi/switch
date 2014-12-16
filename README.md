#Switch
Switch is an easy way to normalize your padding, margins, colors, font sizes in your projects.
It allows you to switch your css direction from left to right to right to left easily.

#Concept
Switch is a set of mixins that map css properties. 
The trick is that you can use a set of predefined "variables" like xs, md, lg, xl, xxl instead of others values.
The other concept is to use the keywords "start" and "end" instead of left and right. 
All the variables are defined in a conf file.

#Installation
###Bower
```bower install switch```
##Npm
```npm install switch```

#Usage:
###Fonts
You can set the font values in the conf file
```scss
.test
{
  @include font-size(xs);
  @include font-size(xxl);
  @include font-size(md);
  @include font-size(13.6px); //you can still use magic numbers ;)
}
```

###Floats
You can set the font values in the conf file
```scss
.test
{
  @include float(start);
  @include float(end);
}
```


###Colors
You can define your custom colors in the conf file
```scss
.test
{
  @include color(success);
  @include background-color(warning);
}
```

###Margins
You can define your margin values in the conf file
```scss
.test
{
  @include margin-top(xs);
  @include margin(xs lg);
  @include margin-start(md);
  @include margin(13px 14px 23px 3px); //you can still use magic numbers ;)
}
```

###Paddings
You can define your padding values in the conf file
```scss
.test
{
  @include padding-top(xs);
  @include padding(xs lg);
  @include padding-start(md);
  @include padding(13px 14px 23px 3px); //you can still use magic numbers ;)
}
```
