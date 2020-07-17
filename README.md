# 作者及联系方式
作者：冰河  
微信：sun_shine_lyz  
QQ：2711098650  
微信公众号： 冰河技术

安装
----
* 确保在你的 AndroidManifest.xml中添加了此项服务
* 在你的class文件中引用此项服务

简单示例
----
```xml
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
         android:versionCode="1"
         android:versionName="1.0">

         <receiver android:name=".MyReceiver" android:enabled="true" android:exported="false">
             <intent-filter>
                 <action android:name="android.intent.action.BOOT_COMPLETED" />
             </intent-filter>
         </receiver>

         <service android:name="com.lyz.mqtt.AMQService" android:exported="false" />

         <uses-permission android:name="android.permission.RECEIVE_BOOT_COMPLETED" />
</manifest>
```


授权声明
-------

    Copyright 2017-2117 binghe
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
    http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

# 扫一扫关注微信公众号

**你在刷抖音，玩游戏的时候，别人都在这里学习，成长，提升，人与人最大的差距其实就是思维。你可能不信，优秀的人，总是在一起。** 
  
扫一扫关注冰河技术微信公众号  
![微信公众号](https://img-blog.csdnimg.cn/20200709131720844.png#pic_center)  
