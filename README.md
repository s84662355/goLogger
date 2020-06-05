##goLogger


##相关的依赖包
- 1、github.com/lestrrat-go/file-rotatelogs
- 2、go.uber.org/zap
- 3、go.uber.org/zap/zapcore

file-rotatelogs 进行日志分割
可以按日分割 ， 按小时分割

##具体应用
import (
    "github.com/s84662355/goLogger"
)

##goLogger.Logger
- 第一个参数是存放日志的目录
- 第二个参数确定是按日分割还是按小时分割
- 返回 *zap.Logger

##按日分割
log := goLogger.Logger("/Users/chenjiahao/GoDemo",true) *goLogger.Log 

##按小时分割
log := goLogger.Logger("/Users/chenjiahao/GoDemo",false) *goLogger.Log 

 
- log.Info(msg string)
- log.Warn(msg string)
- log.Error(msg string)
- log.Debug(msg string)
- log.DPanic(msg string)
- log.Panic(msg string)
- log.Fatal(msg string)


##格式如下
2020-05-26 21:42:25	INFO	log/logger.go:19	操作成功

 



