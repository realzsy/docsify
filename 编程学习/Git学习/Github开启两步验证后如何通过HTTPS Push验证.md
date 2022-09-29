# Github开启两步验证后如何通过HTTPS Push验证

## 两步验证后本地无法使用密码验证
当在Github开启两步验证以后，在本地进行HTTPS Push验证的时候使用登陆密码和两步验证密码都是无法验证，均会提示验证错误。

## 解决办法：Personal access token（个人访问令牌）替代密码验证
通过[Generate new token](https://github.com/settings/tokens)此链接生成新的个人访问令牌

## 验证
用户名：原用户名
密码：上面生成Personal access token