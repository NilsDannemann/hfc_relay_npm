![alt tag](https://dl.dropboxusercontent.com/u/7534528/HFC/Relay/relay_logo.jpg)

# HFC Relay Framework
HFC Relay Framework (SCSS)

<br><hr>
## Installation

####1. Install<br>
Install the npm package from your console.
```sass
npm install hfc-relay --save-dev
```

####2. Create config<br> 
Create a `_hfc-relay-config.scss` with [this content](src/_hfc-relay-config.scss) (but remove all the `!default` statements) <br>

In there you can now:
- safely override any defaults
- easily import/use different fonts 
- toggle features like `$devmode-breakpoints`


####3. Import<br> 
Import both Files in your sass in this order.
```sass
// HFC Relay
@import 'path/to/your/hfc-relay-config.scss';
@import 'node_modules/hfc-relay/hfc-relay.scss';

// Your other imports below
```

That's it. <br>
Happy coding.


<br><hr>
## Usage

#### Layout
- [The Grid](docs/grid.md)
- [Mediaqueries](docs/mediaqueries.md)
- [Quantityqueries](docs/quantityqueries.md)

#### Helpers
- [Container](docs/container.md)
- [Position](docs/position.md)
- [Arrow](docs/arrow.md)
- [Button](docs/button.md)
- [Icon](docs/icon.md)
- [Overlay](docs/overlay.md)
