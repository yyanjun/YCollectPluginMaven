# YCollectPluginMaven

### 1. Gradle集成
(1)`project`的`build.grade`中添加`maven`地址和`classpath`

```java
buildscript {
   repositories {
        jcenter()
        maven {
            url "https://raw.githubusercontent.com/yyanjun/YCollectPluginMaven/master"
        }
    }
    dependencies {
        ...
        classpath 'com.collect.plugin:collect_gradle_plugin:1.0.0'
        ...
    }
}
```
(2)`app`的`build.grade`中添加
	
	// 引用远程maven仓库的插件
    apply plugin: 'com.collect.plugin'
