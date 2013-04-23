# monitor

---

支付宝前端监控脚本。

前端监控脚本可以自动收集页面中未捕获的 JavaScript 异常。
对于已被捕获的异常，可以通过 `monitor.error()` 接口进行监控。

---

## 使用说明

```javascript
try{
  throw new Error("msg");
}catch(ex){
  monitor.error(ex);
}
```


## API

### monitor.log(String productLine, String product, String code)

### monitor.error(Error error)

### monitor.time(String profile, Number value)

### monitor.timeStart(String profile)

### monitor.timeEnd(String profile)
