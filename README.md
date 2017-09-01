# Accordion
Very light and simple module. With the module you can create accordion on your website, useful for creating FAQ lists.

## Version
v2.1.0

## Usage

###### Include files
```html
<link rel="stylesheet" href="css/accordion.css"> 
<script src="js/accordion.min.js"></script>  
```

###### Create HTML layout
```html
<div class="accordion-container">
	<div class="ac">
	    <a href="#" class="ac-q">Lorem ipsum</a>
	    <div class="ac-a">
	        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam quis lacinia nibh.</p>
	    </div>
	</div>

	<div class="ac">
	    <a href="#" class="ac-q">Lorem ipsum</a>
	    <div class="ac-a">
	        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam quis lacinia nibh.</p>
	    </div>
	</div>	

	<div class="ac">
	    <a href="#" class="ac-q">Lorem ipsum</a>
	    <div class="ac-a">
	        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam quis lacinia nibh.</p>
	    </div>
	</div>
</div>
```

###### Initialize the module
```
<script>
	var accordion = new Accordion('accordion-container');	
</script>
```

## API

###### Example
You can initialize more than one accordion per page.
```
<script>
	// Default options
	var accordion = new Accordion('container-first');	

	// User options
	// ( 'container-name', {option: value} )
	var accordion = new Accordion('container-second', {
		duration: 500,
		showFirst: true
	});	
</script>
```

###### Options

| Option  | Type | Default value | Description |
| ----- | ----- | ----- | ----- |
| duration | number | 600 | Animation duration in ms |
| closeOthers | boolean | true | Show only one element at the same time |
| showFirst | boolean | false | Always show first element |
| elClass | string | 'ac' | Element class |
| qClass | string | 'ac-q' | Question class |
| aClass | string | 'ac-a' | Answer class |