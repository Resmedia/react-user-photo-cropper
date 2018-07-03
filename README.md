## Installation

In your project

```shell
npm install --save react-user-photo-cropper

or 

yarn add react-user-photo-cropper
```
react-user-photo-cropper need depends react-bootstrap for modal functionality.

```shell
react and react-bootstrap
```

## Usage

Usage is fairly simple, you can check the /example folder on github for a slightly more complex use 
case (the use case you see above in the demo). AvatarCropper simple takes a width and a height to 
determine what size avatar you would like. AvatarCropper then takes an image property where you can 
pass an external image, a user uploaded data URI or whatever you would like. An onRequestHide 
function is passed to the underlying modal so you can decide how to dismiss the modal. Lastly onCrop 
callback function is required, and gives you back the cropped Image, for you to do with as you wish.

```$xslt
import AvatarCropper from 'react-avatar-cropper'

return (
          <AvatarCropper
             modalTitle="Переместить и обрезать"
             onRequestHide={this.handleRequestHide}
             onCrop={this.handleCrop}
             cropperOpen={this.state.cropperOpen}
             image={this.state.image}
             width={600}
             height={600}
             modalSize="sm"
             closeButtonCopy="Отмена"
             cropButtonCopy="Сохранить"
           />
      );
```

This clone of http://dropsofserenity.github.io/react-avatar-cropper/ look there for more examples and info.
