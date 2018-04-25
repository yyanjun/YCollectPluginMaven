# YCollectPluginMaven

### 1. Gradle集成
`project`的`build.grade`中添加`maven`地址和`classpath`
+
+    buildscript {
+    repositories {
+        jcenter()
+        maven {
+            url "git@github.com:yyanjun/YCollectPluginMaven/master"
+        }
+    }
+    dependencies {
+        ...
+        classpath 'com.collect.plugin:YCollectPluginn:1.0.0'
+        ...
+    }

`app`的`build.grade`中添加
	
	// 引用远程maven仓库的插件
    apply plugin: 'com.collect.plugin'
