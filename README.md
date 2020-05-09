# goLogger

使用了
	github.com/lestrrat-go/file-rotatelogs
	go.uber.org/zap
	go.uber.org/zap/zapcore

file-rotatelogs 进行日志分割
可以按日分割 ， 按小时分割

import (
    "github.com/s84662355/goLogger"
)


第一个参数是存放日志的目录
第二个参数确定是按日分割还是按小时分割

返回 *zap.Logger

按日分割
goLogger.Logger("/Users/chenjiahao/GoDemo",true)

按小时分割
goLogger.Logger("/Users/chenjiahao/GoDemo",false)
