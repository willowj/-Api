### ip.taobao

​	get self ip : <http://httpbin.org/ip>


1. 请求接口（GET）：

     `http://ip.taobao.com/service/getIpInfo.php?ip=[ip地址字串]`

     > eg:	   http://ip.taobao.com/service/getIpInfo.php?ip=113.66.41.17


2. 响应信息：

   （json格式的）国家 、省（自治区或直辖市）、市（县）、运营商

   ​

3. 返回数据格式：

   > ~~~json
   > {
   >     "code": 0,
   >     "data": {
   >         "country": "\u4e2d\u56fd",  // 国家
   >         "country_id": "CN",
   >
   >         "area": "\u534e\u5357",     // 区域 (华南/..etc)
   >         "area_id": "800000",
   >
   >         "region": "\u5e7f\u4e1c\u7701", // 省
   >         "region_id": "440000",
   >
   >         "city": "\u5e7f\u5dde\u5e02", // 市
   >         "city_id": "440100",
   >
   >         "county": "",               // 区/县
   >         "county_id": "-1",          // -1 表示该项查询失败
   >
   >         "isp": "\u7535\u4fe1",      // 运营商
   >         "isp_id": "100017",
   >         
   >         "ip": "113.66.41.17"
   >     }
   > }
   > ~~~

   其中code的值的含义为，0：成功，1：失败。

   >  from : [ip.taobao](http://ip.taobao.com/instructions.php)

   ​

   ​
