# @ddatabase/session

Make a session from a dDatabase that can auto cancel all inflight requests / downloads.

```
npm install @ddatabase/session
```

## Usage

``` js
const DDatabase Session = require('@ddatabase/session')

const session = new DDatabase Session(feed)

// get a block
const block = await session.get(42)

// get a bunch of blocks
await session.download({ start: 0, end: 42 })

// cancel all currently inflight
session.cancel()
```

## License

MIT
