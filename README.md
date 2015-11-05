React Lazy Load Component
=========================

Really simple component that renders children elements when they enter the viewport.

[![npm downloads](https://img.shields.io/npm/dm/react-lazy-load.svg?style=flat-square)](https://www.npmjs.com/package/react-lazy-load)

## Install

```
npm install --save react-lazy-load
```

## Usage

```jsx
import React from 'react';
import LazyLoad from 'react-lazy-load';

class MyComponent {
  render() {
    return (
      <LazyLoad>
        <div>some content</div>
      </LazyLoad>
    );
  }
}
```

## Props

### height={String|Number}

This is used to set the elements height even when it contains no content.

```jsx
<LazyLoad height={100}>
  <div>some content</div>
</LazyLoad>
```

### threshold={Number}

By default images are loaded when they appear on the screen. If you want images to load earlier use threshold parameter. Setting threshold to 200 causes image to load 200 pixels before it appears on viewport.

```jsx
<LazyLoad threshold={200}>
  <div>some content</div>
</LazyLoad>
```