# sast2023 word game

## 环境配置

目前没有第三方依赖项

## 使用设置

约定以下参数：

```
--file  -f  接文章的路径
--choosse -c 接选择文章的名称，若未输入或找不到名字，则随机选择
```


文章使用 JSON 存储，的格式如下：
```
{
    "language": "zh",
    "articles": [
        {
            "title": "贵系日常",
            "article": "我们都爱{{1}}这门课程。这门课程是多么的{{2}}，以至于所有人都在课程上认真地{{3}}。在设计数字电路时,我们需要运用到逻辑门、半导体存储器等知识。这些内容相互联系,共同构成复杂的数字电路。这门课能启发我们的逻辑思维能力和科学思考能力。通过为难我们的练习和作业,我们的理解能力和解决问题的能力得到了提高。这些将对今后的{{4}}和工作有很大益处。",
            "hints": ["教材名称", "形容词", "动词，与学生相关", "你最喜欢做的事情"]
        }
    ]
}
```
可以通过以下指令进入游戏
```shell
python main.py -f <json文件路径> (-c <"所选文章名字">)
#在此文件夹目录下，可通过如下命令进入游戏：
python main.py -f example.json
```

