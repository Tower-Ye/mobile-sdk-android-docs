# 帐号模块 Account
## 登出接口

* 接口说明：登出接口，清除 SDK 中的 token、userId 等缓存数据。

**示例代码：**

```java
RokidMobileSDK.account.logout(new ILogoutResultCallback() {
    @Override
    public void onLogoutSucceed() {
        Logger.d("onLogoutSucceed is called.");
        ... // do something
    }

     @Override
    public void onLogoutFailed(String errorCode, String errorMsg){
        Logger.e("onLogoutFailed errorCode=" + errorCode + " errorMsg=" + errorMsg);
        ... // do something
    }
});
```



