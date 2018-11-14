##比特之家APP接口

接口传输方式 `RPC`

## 接口列表
- [APP版本更新](#APP版本更新)


------------------

接口地址
> 域名/cms/bhouse.php?c=index

请求方式
> post

参数类型(`Content-Type`)
> application/json


## APP版本更新

##### 请求参数

    {
        "jsonrpc":"2.0",
        "method":"appUp",
        "params":[
            {
                "system":"android", //系統
                "version":"1.1.0",  //旧版本
                "ver_num":"11", //内
                "channel":"huawei/appstore"  //下
            }
        ],
        "id":1
    }


##### 返回结果

  成功：
  
    {
        "jsonrpc": "2.0",
        "result": {
            "code": 0,
            "message": "success",
            "data": {
                "url": "http://**********.apk",    //新版本下载地址
                "message": "版本上线了", //消息内容
                "version": "V1.0.1",    //
                "is_update": "0",   //是
                "is_examine": "1",  //
                "ver_num": "1111",  //
                "is_open": "0"  //
            }
        },
        "id": 1
    }