# bubble-picker

## Getting started

`$ npm install bubble-picker`

### Mostly automatic installation (RN < 0.60)

## Usage

```javascript
import { BubblePicker } from "bubble-picker";
//...
onBubblePress = e => {
  const { isSelected, id } = e;
  // Do stuff to save the set the bubble as selected
};
//...
const items = ["Option 1", "Option 2", "Option 3"].map(name => ({
  text: name,
  color: "#888888",
  textColor: "#ffffff",
  isSelected: selectled.indexOf(x.id) > -1,
  id: name
}));
const PickerProps = Platform.select({
  android: {
    radius: 1,
    fontSize: 16
  },
  ios: {
    radius: 70,
    fontSize: 16
  }
});
// rendering:
<BubblePicker
  {...PickerProps}
  items={items}
  onPress={this.onBubblePress}
/>;
```
