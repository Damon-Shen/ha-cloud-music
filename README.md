# 网易云音乐HASS插件

基于第三方UI修改，配合自定义的media插件实现的后台播放功能；

> custom_components：对应的HomeAssistant自定义插件目录

> 这个前端的播放器由 [maomao1996](https://github.com/maomao1996) 开发，我只是基础上进行了修改

## 免责声明
本站音频文件来自各网站接口，本站不会修改任何音频文件

音频版权来自各网站，本站只提供数据查询服务，不提供任何音频存储和贩卖服务

本项目仅为自己测试项目，请勿用作商业用途，请勿通过本项目下载盗版歌曲资源，否则后果自负！

## 如何使用

> 安装

1.（建议）使用[HACS安装](https://github.com/custom-components/hacs)

在HACS里输入：https://github.com/shaonianzhentan/ha-cloud-music 即可安装成功（类型选择Integration）

2.自定义安装

将本项目custom_components里的内容，放到HASS的custom_components文件夹中

> 后台插件配置

然后在configuration.yaml中配置以下内容
```
media_player:
  - platform: ha-cloud-music

```

# 请一定要在HomeAssistant里使用，不然没啥用

## 功能

- 播放器
- 快捷键操作
- 歌词滚动
- 正在播放
- 排行榜
- 歌单详情
- 搜索
- 播放历史
- 查看评论
- 同步网易云歌单

## 界面欣赏

PC端界面自我感觉还行， 就是移动端界面总觉得怪怪的，奈何审美有限，所以又去整了高仿网易云的 React 版本（如果小哥哥、小姐姐们有好看的界面，欢迎交流哈）

### PC

#### 选择媒体插件
![选择媒体插件](https://raw.githubusercontent.com/shaonianzhentan/lovelace-cloud-music/master/screenshots/select_mode.png)
#### 正在播放
![正在播放](https://raw.githubusercontent.com/maomao1996/Vue-mmPlayer/master/screenshots/1.jpg)
#### 排行榜
![排行榜](https://raw.githubusercontent.com/maomao1996/Vue-mmPlayer/master/screenshots/2.jpg)
#### 搜索
![搜索](https://raw.githubusercontent.com/maomao1996/Vue-mmPlayer/master/screenshots/3.jpg)
#### 我的歌单
![我的歌单](https://raw.githubusercontent.com/maomao1996/Vue-mmPlayer/master/screenshots/4.jpg)
#### 我听过的
![我听过的](https://raw.githubusercontent.com/maomao1996/Vue-mmPlayer/master/screenshots/5.jpg)
#### 歌曲评论
![歌曲评论](https://raw.githubusercontent.com/maomao1996/Vue-mmPlayer/master/screenshots/6.jpg)

### 移动端

![移动端一](https://raw.githubusercontent.com/maomao1996/Vue-mmPlayer/master/screenshots/7.jpg)
![移动端二](https://raw.githubusercontent.com/maomao1996/Vue-mmPlayer/master/screenshots/8.jpg)

## 更新说明
### V1.0.0（2019.09.25）
- 将前端播放器和插件集成到一起（安装更简单）
- 解决flac无法播放不能跳到下一曲的问题
- 解决歌词显示不同步的问题
- 修复自动播放下一曲的逻辑问题
- 注释了调试日志

### V0.0.1（2019.07.06）
- 解决后台播放支持全部媒体插件的功能

## 其他说明

- 并没有全面测试，所以可能有BUG
- 如有问题请直接在 Issues 中提，或者您发现问题并有非常好的解决方案，欢迎 PR

## License

[MIT](https://github.com/maomao1996/Vue-mmPlayer/blob/master/LICENSE)
