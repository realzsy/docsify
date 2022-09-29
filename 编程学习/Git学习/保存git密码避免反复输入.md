# 保存git密码避免反复输入

在本地提交代码的时候每次都要输入用户名和密码，通过以下代码可以保存git验证的用户名和密码

```bash
git config --global credential.helper store
```
> [!tip]
> 上面的代码是永久保存密码

若是想要在一定时间内保存，可以参考一下代码：

<code>默认保存15分钟</code>

```bash
git config --global credential.helper cache
```
<code>可自定义保存时间（单位：秒）</code>

```bash
git config credential.helper 'cache --timeout=3600'
```