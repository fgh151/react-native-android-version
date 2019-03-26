React Native Android Styles
===

This package allow to apply styles to specific android version.

Installation
---

```
npm i --save react-native-android-version
```
or
```
yarn add react-native-android-version
```


Example Usage
---

``` js

import AndroidVersion from "react-native-android-version";
import {StyleSheet} from "react-native";


const styles = StyleSheet.create({
    image: {
        ...AndroidVersion.select({
        
        //Apply styles to android api 28 and hight
        
            '>=26': {
                width: 'auto',
                height: 'auto',
            },
            
        //Apply styles to android api 28
            
            
            '28': {
                width: 'auto',
                height: 'auto',
            },
            
        //Apply styles to android api 25
        
            25: {
                width: 'auto',
                height: 'auto',
            },
            
        //Styles for other android api levels
        
            default: {
                width: '100%',
                height: '100%',
            }
        })
    }
});
```

Contribute
---

Of course, contributions welcomed! 🙌

License
---

[MIT](http://cheeaun.mit-license.org/).
