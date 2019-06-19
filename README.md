![Build Status](https://drone.dayler.dev/api/badges/iknpx/feather-react/status.svg)
[![npm version](https://badge.fury.io/js/feather-react.svg)](https://badge.fury.io/js/feather-react)
[![Downloads](http://img.shields.io/npm/dm/feather-react.svg?style=flat)](https://npmjs.org/package/feather-react)

# feather-react
Simple way to start using `feater-icons` as React component

### Installation
```bash
npm install --save feather-react
```

### Usage
Children prop can be used as one of icon name from [feathericons.com](https://feathericons.com/)

```javascript
import Icon from 'feather-react'

const MyComponent = () => {
    return <Icon>feather</Icon>
}
```

Will return ![feather](https://iknpx.github.io/feather-react/feather.svg)

### Icons Source
```javascript
import { source } from 'feather-react'

source === {
    icons: [{
        id: 1,                   // random number
        name: 'activity',        // actual name provided by feather-icons
        tags: ['pulse', '...'],  // tags list  provided by feather-icons
    }],
    list: ['activity', '...'],   // array of icons names
}

```

### Props Api
```javascript
{
    // icon name (`x` by default)
    children: PropTypes.oneOf(source.list).isRequired,
    // icon size, will be as width/height props of root <svg> (24 by default)
    size: PropTypes.number,
}
```

---

:heart: Thanks [StdLib](https://stdlib.com) for your essential work with Feathericons
