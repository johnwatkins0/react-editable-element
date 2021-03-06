# react-editable-html-element

Allows HTML elements to be modified in place by changing them into inputs when clicked.

[Examples](https://johnwatkins0.github.io/react-editable-html-element/example/)

## Install

```
npm install react-editable-html-elements
```

```
yarn add react-editable-html-elements
```

## Usage

```javascript
import React from 'react';
import EditableElement from 'react-editable-html-element';

const YourComponent = () => {
  const yourProps = {
    // See Props section
  };

  return <EditableElement {...yourProps} />;
};
```

## Props

| Name             | Type                                                       | Description                                           | Default                                |
| ---------------- | ---------------------------------------------------------- | ----------------------------------------------------- | -------------------------------------- |
| allowEditing     | bool                                                       | Set to false to disable editing completely.           | true                                   |
| editable         | bool                                                       | Should the element be editable when mounted?          | false; true if the value prop is empty |
| element          | string (see src/htmlTags.js for the allowed HTML elements) | The HTML element.                                     | 'div'                                  |
| elementClassName | string                                                     | CSS class(es) to apply to the element.                | ''                                     |
| elementStyle     | object                                                     | React-formatted CSS to apply to the element.          | {}                                     |
| inputClassName   | string                                                     | CSS classes(es) to apply to the input.                | ''                                     |
| inputStyle       | object                                                     | React-formatted CSS to apply to the input.            | {}                                     |
| onChange         | function                                                   | Override the component's built-in input change.       | null                                   |
| onKeyDown        | function                                                   | Override the component's built-in onKeyDown function. | null                                   |
| placeholder      | string                                                     | Text to display when the input is empty.              | 'Enter text'                           |
| value            | string                                                     | The value of the element/input.                       | ''                                     |
