# vue-kityminder-editor

## use

`npm install vue-kityminder-editor-v2 --save`

## main.js
```js
import kityminder from 'vue-kityminder-editor-v2'

Vue.use(kityminder);
```
## **.vue
```js
    <minder
      v-for="(item,index) in importData" 
      :key="index"
      :importData="item"
      :index='index'
      @exportData="exportData"
    ></minder>
```

```js
importData: [
    { 
        "data": { "text": "新闻1", "id": 2, "priority1": 1 },
        "children": [
            { 
                "data": { "text": "新闻2", "id": 3, "priority1": 1 },
                "children": [
                    { "data": { "text": "新闻3", "id": 4, "priority1": 1 }},
                    { "data": { "text": "网页4", "id": 5, "priority1": 1 } },
                    { "data": { "text": "贴吧5", "id": 6, "priority1": 2 } },
                    { "data": { "text": "知道6", "id": 7, "priority1": 3 } },
                    { "data": { "text": "音乐7", "id": 8, "priority1": 4 } }
                ]
            },
            { "data": { "text": "网页8", "id": 9, "priority1": 1 } },
            { "data": { "text": "贴吧9", "id": 10, "priority1": 2 } },
            { "data": { "text": "知道11", "id": 11, "priority1": 3 } },
            { "data": { "text": "音乐12", "id": 12, "priority1": 4 } }
        ]
    },
    { 
        "data": { "text": "新闻1", "id": 2, "priority1": 1 },
        "children": [
            { "data": { "text": "贴吧9", "id": 10, "priority1": 2 } },
            { "data": { "text": "知道11", "id": 11, "priority1": 3 } },
            { "data": { "text": "音乐12", "id": 12, "priority1": 4 } }
        ]
    },
    { 
        "data": { "text": "新闻1", "id": 2, "priority1": 1 },
        "children": [
            { 
                "data": { "text": "新闻2", "id": 3, "priority1": 1 },
                "children": [
                    { "data": { "text": "新闻3", "id": 4, "priority1": 1 }},
                    { "data": { "text": "网页4", "id": 5, "priority1": 1 } },
                    { "data": { "text": "贴吧5", "id": 6, "priority1": 2 } },
                    { "data": { "text": "知道6", "id": 7, "priority1": 3 } },
                    { "data": { "text": "音乐7", "id": 8, "priority1": 4 } }
                ]
            },
            { "data": { "text": "网页8", "id": 9, "priority1": 1 } },
            { "data": { "text": "贴吧9", "id": 10, "priority1": 2 } },
            { "data": { "text": "知道11", "id": 11, "priority1": 3 } },
            { "data": { "text": "音乐12", "id": 12, "priority1": 4 } }
        ]
    }
]
```
