#作者简介: 
刘亚壮，高级软件架构师，Java编程专家，开源分布式消息引擎Mysum发起者、核心架构师及开发者，国内知名开源分布式数据库中间件Mycat核心架构师、开发者，精通Java, C, C++, Python, Hadoop大数据生态体系，熟悉MySQL、Redis内核，Android底层架构。多年来致力于分布式系统架构、微服务、分布式数据库、大数据技术的研究，曾主导过众多分布式系统、微服务及大数据项目的架构设计、研发和实施落地。在高并发、高可用、高可扩展性、高可维护性和大数据等领域拥有丰富的经验。对Hadoop、Spark、Storm等大数据框架源码进行过深度分析并具有丰富的实战经验。

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

    Copyright 2017-2117 liuyazhuang
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
    http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
