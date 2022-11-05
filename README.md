# SB2.0 使用，叉回來確保版本穩定，勿改勿刪

## fork from @gpsgate/react-native-eventsource

@gpsgate/react-native-eventsource

### Installation

```
npm i git+https://github.com/a0921313520/react-native-eventsource.git
```

### Usage

```js
import EventSource from "@gpsgate/react-native-eventsource";

const url = "https://domain/sse";
const eventSource = new EventSource(url);
eventSource.onopen = () => {
  console.debug("onopen");
};
eventSource.onmessage = message => {
  console.debug(message);
};
eventSource.onerror = err => {
  console.error(err);
};
```
