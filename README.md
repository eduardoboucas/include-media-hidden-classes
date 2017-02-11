<a href="http://include-media.com">!['At' sign](http://include-media.com/assets/images/logo.png)</a>

# include-media — Hidden classes plugin

> Get **include-media** [here](https://github.com/eduardoboucas/include-media).

### Introduction

This plugin generates a set of classes that allow elements to be hidden for specific breakpoints, as per [this issue](https://github.com/eduardoboucas/include-media/issues/109#issuecomment-279157208).

*Example:*

```scss
/* Hidden for viewports on the "phone" breakpoint
.hidden--for-phone

/* Hidden for viewports larger than the "phone" breakpoint (inclusive)
.hidden--from-phone

/* Hidden for viewports smaller than the "phone" breakpoint (inclusive)
.hidden--to-phone
```

### Configuration

> `$im-hidden-class`: The name of the generated classes (default: `hidden`)