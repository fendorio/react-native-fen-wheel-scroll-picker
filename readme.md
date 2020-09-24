## Changes since fork

-   Added 'displayField' property, where you can pass in an object key (single level) to render, this is useful if you want to pass in an array of objects, and want to render one of the fields.
-   Added 'fontSize' and 'lineHeight' prop, to allow further customisation of the text element rendered inside each option.

This has not been tested since 2019.

## react-native-wheel-scroll-picker

a pure js picker, each option item customizable

![example](./demo/test.gif)

### usage

```shell
npm install react-native-fen-wheel-scroll-picker --save
```

```jsx
import React, { Component } from "react";
import ScrollPicker from "react-native-fen-wheel-scroll-picker";

export default class SimpleExample extends Component {
    render() {
        return (
            <ScrollPicker
                dataSource={["a", "b", "c", "d"]}
                selectedIndex={1}
                renderItem={(data, index, isSelected) => {
                    //
                }}
                onValueChange={(data, selectedIndex) => {
                    //
                }}
                wrapperHeight={180}
                wrapperWidth={150}
                wrapperBackground={"#FFFFFF"}
                itemHeight={60}
                highlightColor={"#d8d8d8"}
                highlightBorderWidth={2}
                activeItemColor={"#222121"}
                itemColor={"#B4B4B4"}
            />
        );
    }
}
```
