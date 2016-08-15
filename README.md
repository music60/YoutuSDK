# YoutuSDK
腾讯优图SDK,人脸识别,身份证OCR识别
#### 腾讯优图SDK
1,由于业务需要对接了下身份证识别信息，腾讯优图身份证识别主要是把图片上传云端，然后云端处理完结果，返回给我们处理完的结果。

腾讯优图SDK接入网址 http://open.youtu.qq.com/

身份证OCRAPI文档 http://open.youtu.qq.com/welcome/developer#/api-summary

该SDK是基于腾讯优图的SDK,直接抽出涉及优图的一些工具类而已，并把youtu设置成单例模式，在application初始化一次即可;

原版SDK网址:https://github.com/Tencent-YouTu/android_sdk

使用方法

##### 初始化

```
 /**
 * String appid, String secret_id, String secret_key
 */
Youtu.initSDK("1000***","***********","**********************");
```

##### 调用身份证识别

```
//bitmap 身份证
//bitmap 0为身份证正面，1为身份证反面
Youtu.getInstance().IdcardOcr(bitmap, 0)
```



License
-------

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.


