# 初学python的一个练手小项目
## 基于DFA算法实现的敏感词屏蔽，运行效率较高
### 功能介绍
- 提供一个字符串，即可得到屏蔽敏感词后的字符串
- 可忽略掉无效字符（汉字、字母、数字以外的符号）
- 提供了重新选择敏感词库以及添加单个敏感词的功能
- 提供了查询字符串是否存在敏感词的功能（不进行屏蔽）
### 文件说明
- dfa.py为源码
- TestDFA.py为使用pytest进行运行性能测试
- sensitive_words.txt为默认敏感词库
- DfaApi.py为建立运行于web上的API接口
    - text_filter/string命令返回是否存在敏感词以及屏蔽后的字符串
    - add_new_words/string命令向敏感词库添加新的敏感词
    - change_text/string命令修改新的敏感词词库，string为新文件的path

项目来源地址：https://github.com/spirit-yzk/sensitive_words_blocking.git
