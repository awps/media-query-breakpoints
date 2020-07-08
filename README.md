### Installation: 
```
@include "~media-query-breakpoints";
```

### Available media query mixins: 
``` 
// Mobile-first
for-phone-up() 
for-tablet-up() 
for-notebook-up() 
for-monitor-up() 
for-2k-up()
for-4k-up()

// Desktop-first
for-phone-down() 
for-tablet-down() 
for-notebook-down() 
for-monitor-down() 
for-2k-down()
for-4k-down()
```

### Usage example: 
``` 
.some-element{
    // Default CSS rules
    // ------------------------
    padding: 10px;
    margin: 20px 0; 

    // Rules for tablet and up
    // ------------------------
    @include for-tablet-up(){
        padding: 30px;
        margin: 40px 0;
    }

    // Rules for notebook and up
    // ------------------------
    @include for-notebook-up(){
        padding: 60px;
        margin: 80px 0;
    }

    // Rules for monitor and up
    // ------------------------
    @include for-monitor-up(){
        margin-bottom: 120px;
    }
}
```

### Override breakpoint values: 
```
$media-bp-phone: 480px;
$media-bp-tablet: 768px;
$media-bp-notebook: 1024px;
$media-bp-monitor: 1280px;
$media-bp-2k: 1920px;
$media-bp-4k: 3840px;

@include "~media-query-breakpoints";
``` 
