# ~~博客卷~~ 友链
~~虽然没有人来互换友链但是还是写了呢 万一有人呢？（被打~~
## 对 ~~制作博客卷的原料~~ 加入友链的站点的要求（？）
- 无侵入性广告
    - 广告是很讨厌的，是吧（）所以最好不要出现侵入性广告这种东西哦（？
- 网站域名是 [Public Suffix List](https://publicsuffix.org/list/public_suffix_list.dat) 的子域
- 要有原创内容
- 差不多就这样了（？
## ~~制作博客卷~~ 交换友链

1. `Fork` 一下这个仓库
3. 在本 `repo` 的 `src/data/friends.js` 中加入一个 `entry`：
```js
{
    name: <站点的名称>,
    href: <站点的 URL>,
    desc: <站点的描述 (你的 Slogan, etc)>,
    logo_href: <想要在展示页面展示的 Logo 的 URL>
}
```
【（`logo` 最好是正方形的哦（而且长和宽最好不要超过 512 px）】

~~处理好的博客卷原料~~ `entry` 示例如下：
```js
{
    name: "鸭鸭省教育科学研究院",
    href: "https://sei.ya/",
    desc: "同学！来做题辣！",
    logo_href: "https://sei.ya/logo@512x512.png"
}
```


3. 发起一个 `Pull Request`
6. 等我 `merge`（ 

### 将本站添加至你的友链页面中
```js
{
    name: "Francie\'s Blog",
    href: "https://blog.francie.cc/",
    desc: "Francie 写奇奇怪怪东西的地方（",
    logo_href: "https://avatars.githubusercontent.com/u/106010535"
}
```

## 结尾
Congratulations! 你会做博客卷辣！（