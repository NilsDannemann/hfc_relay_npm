# HFC Relay Framework
HFC Relay Framework (SCSS)

<br><hr>
## Installation

####1. Install<br>
Install the npm package from your console.
```sass
npm install hfc-relay --save-dev
```

####2. Create config File<br> 
Create a `config.scss` with [this content](src/_config.scss). <br>

In there you can now:
- import/use different fonts 
- safely override any defaults
- toggle features like `$devmode-breakpoints`


####3. Import Files<br> 
Import both Files.
```sass
// HFC Relay - Main File
@import 'node_modules/hfc-relay/src/hfc-relay.scss';
// HFC Relay - Your config File
@import 'path/to/config.scss';
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
