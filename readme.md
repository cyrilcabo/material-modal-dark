# Material Modal Dark

## Installation

* Run `npm install material-modal-dark` in your project.
* Import in your project using `import Modal from 'material-modal-dark';`

## Usage

`<Modal {...props} />`

## Props

* **dark** (`optional` **|** `boolean` **|** `default:false`) - enables the dark mode of the modal
* **open** (`required` **|** `boolean` **|** `default:false`) - state if the modal should be open or not
* **handleClose** (`required` **|** `function` **|** `default:null`) - fires when the component should close
* **children** (`required` **|** `JSX.Element` **|** `default:''`) - the content of the modal

## Sample Usage
```JSX
import React from 'react';
import Modal from 'material-modal-dark;


const Component = () => {
	const [open, setOpen] = React.useState(false);
	const handleOpen = () => setOpen(true);
	const handleClose = () => setOpen(false);
	return (
		<React.Fragment>
			<button onClick={handleOpen}> Open Modal </button>
			<Modal handleClose={handleClose} open={open} dark={true}>
				<h1> Hi I am a modal </h1>
			</Modal>
		</React.Fragment>
	);
}


export default Component;
```

## Demo

### Web view:
![Demo web view](https://drive.google.com/uc?export=view&id=1lKl9o8Z0SCm0vxMOO49nw8yWo0jBywJ2)

### Mobile view:
![Demo mobile view](https://drive.google.com/uc?export=view&id=1jKwsgedqj822F-bztfE9XkCyC235NPRH)