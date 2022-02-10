# gdc-component-modal

This package is a part of the project 14 of the OpenClassrooms "Front End Developer" courses.
For this one I had to turn an old JQuery website into a full react app.

If you want to see the rest of the project it's right there : https://github.com/Gautier-DC/GautierDeConinck_14_07012022

We had 4 differents options and I choose to make a react modal component as an npm package.

You can find on npm here : https://www.npmjs.com/package/gdc-component-modal

Now that you have the context, how does it works ?

## Requirements

First of all you need to install Node.js v14.15.4 or latest version.
You also need to have react and react-dom v17.0.2 or latest in your project if you want to run it.

## Installation

In your project, run the following command :

`npm install gdc-component-modal`

So now you have access to the modal component, you can add it to your project, for example like that :

```<div className="App">
        <button onClick={() => setShow(true)}>Show Modal</button>
        <Modal title="New Modal" onClose={() => setShow(false)} show={show}>
            <p>Modal incredible content 👽</p>
        </Modal>
    </div>
```

So you can custom Modal with the title props and in the children part you can put anything you want: simple paragraph, formular, images, button...

**One last important thing :**
you need to define the following useState `const [show, setShow] = useState(false);` where you use the component in order to make it work.
Without it you will not be abble to display the modal !

## Used Technologies / Dependencies

- React :
  - react
  - react-dom
  - react-transition-group
- postcss v8.0
- babel
- rollup
