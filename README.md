# Blank-Settings-Utils
 A utility to create blank settings tab
# How to use

in index.js file, add this code

```javascript
import { settingsUtils } from "https://unpkg.com/blank-settings-utils@latest/Settings-Utils.js"

let data = [
    {
        "groupName": '',         // String
        "titleKey": '',          // String, must start with "el_"
        "titleName": '',         // String
        "capitalTitleKey": '',   // String
        "capitalTitleName": '',  // String
        "element": [
            {
                "name": "",      // String
                "title": "",     // String, must start with "el_"
                "titleName": "", // String
                "class": "",     // String
                "id": "",        // String 
            },
        ],
    },
]

export function init(context) {
    settingsUtils(context, data)
}
```

# Example

```javascript
import { settingsUtils } from "https://unpkg.com/blank-settings-utils@latest/Settings-Utils.js"

let data = [
    {
        "groupName": 'test',
        "titleKey": 'el_test',
        "titleName": 'Test',
        "capitalTitleKey": 'el_test_capital',
        "capitalTitleName": 'TEST',
        "element": [
            {
                "name": "el-test-settings",
                "title": "el_test-settings",
                "titleName": "TEST SETTINGS",
                "class": "test_settings",
                "id": "testSettings",
            }
        ],
    },
]

export function init(context) {
    settingsUtils(context, data)
}
```

- This will create a "test" group and "test" tab in settings

![image](https://github.com/Elaina69/Blank-Settings-Utils/assets/94338907/d3ca842f-3d2c-41e8-9439-e2afa35dc912)


- You also can add more groups and tabs as you want

```javascript
import { settingsUtils } from "https://unpkg.com/blank-settings-utils@latest/Settings-Utils.js"

let data = [
    {
        "groupName": 'test',
        "titleKey": 'el_test',
        "titleName": 'Test',
        "capitalTitleKey": 'el_test_capital',
        "capitalTitleName": 'TEST',
        "element": [
            {
                "name": "el-test-settings",
                "title": "el_test-settings",
                "titleName": "TEST SETTINGS",
                "class": "test_settings",
                "id": "testSettings",
            }
        ],
    },
    {
        "groupName": 'test2',
        "titleKey": 'el_test2',
        "titleName": 'Test 2',
        "capitalTitleKey": 'el_test_capital2',
        "capitalTitleName": 'TEST 2',
        "element": [
            {
                "name": "el-test-settings2",
                "title": "el_test-settings2",
                "titleName": "TEST SETTINGS 2",
                "class": "test_settings2",
                "id": "testSettings2",
            },
            {
                "name": "el-test-settings3",
                "title": "el_test-settings3",
                "titleName": "TEST SETTINGS 3",
                "class": "test_settings3",
                "id": "testSettings3",
            }
        ],
    },
]

export function init(context) {
    settingsUtils(context, data)
}
```
