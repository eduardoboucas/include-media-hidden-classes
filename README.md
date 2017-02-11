<a href="http://include-media.com">!['At' sign](http://include-media.com/assets/images/logo.png)</a>

# include-media — Hidden classes plugin

> Get **include-media** [here](https://github.com/eduardoboucas/include-media).

### Introduction

This plugin generates a set of classes that allow elements to be hidden for specific breakpoints, as per [this issue](https://github.com/eduardoboucas/include-media/issues/109#issuecomment-279157208).

*Example:*

```scss
/* Hidden for viewports on the "phone" breakpoint */
.hidden--for-phone

/* Hidden for viewports larger than the "phone" breakpoint (inclusive) */
.hidden--from-phone

/* Hidden for viewports smaller than the "phone" breakpoint (inclusive) */
.hidden--to-phone
```

*Generates:*

```scss
@media (min-width: 320px) and (max-width: 767px) {
  .hidden--for-phone {
    display: none;
  }
}
@media (min-width: 320px) {
  .hidden--from-phone {
    display: none;
  }
}
@media (max-width: 319px) {
  .hidden--to-phone {
    display: none;
  }
}
@media (min-width: 768px) and (max-width: 1023px) {
  .hidden--for-tablet {
    display: none;
  }
}
@media (min-width: 768px) {
  .hidden--from-tablet {
    display: none;
  }
}
@media (max-width: 767px) {
  .hidden--to-tablet {
    display: none;
  }
}
@media (min-width: 1024px) {
  .hidden--for-desktop {
    display: none;
  }
}
@media (max-width: 1023px) {
  .hidden--to-desktop {
    display: none;
  }
}
```

### Configuration

> `$im-hidden-class`: The name of the generated classes (default: `hidden`)