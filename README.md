## background

产研业务数据会有级联表(Cascade)的形式，实际上是简单的树结构，例如`省-市-区-县-乡`的选择

这些数据用excel整理。但开发使用时，一般录入json。对于没有维护工具的团队来说，各方对接比较麻烦

产品经理将excel另存为csv后，可以使用本脚本转化为json

## data structure

```json
// json data structure:
{
    {
        "name":"option-name",
        "value":"business-id",
        "children":[]
    }
}
```

## requirements

- python3
- jupyter-notebook