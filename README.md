# foodwake

食物营养成分表，共 1643 条数据。

原始数据来自：[https://www.foodwake.com/](https://www.foodwake.com/)。

[guyongjie/foodwake](https://github.com/guyongjie/foodwake) 对 foodwake 进行了爬取，我使用并修改了他的数据文件 `data.json`、`new_data.json`，感谢！

- 新增了 `type` 字段，为食物的类别，其值为如下一种：
```
谷类 薯类 豆类 蔬菜 菌类 藻类 水果 坚果
畜肉 禽肉 乳类 蛋类 河海鲜
茶类 酒类 油类 调味品类 零食饮料
```

- 新增了 `imgUrl` 字段，其值为提取自 [shutterstock 图库](https://www.shutterstock.com/zh/) 的相关图片地址。

  注意：并不是所有食物都有图片，并不是所有图片都与食物有强相关性！最好大概浏览一篇。

- 例子：
```
{
  "name": "蔓越莓汁鸡尾酒",
  "url": "http://www.foodwake.com/food/1059",
  "info": {
    "能量":"54千卡",
    "蛋白质":"克",
    "脂肪":"0.1克",
    "碳水化合物":"13.52克",
    "粗纤维":"克",
    "单不饱和脂肪酸":"0.019克",
    ...
  },
  "nickname": "蔓越莓汁鸡尾酒，瓶装（U）",
  "type": "酒类",
  "update_time": 1604314208042,
  "imgUrl": "https://image.shutterstock.com/image-photo/fresh-cranberry-drink-on-wooden-260nw-178274312.jpg"
}
```
