# Android-Hello-World
只是一个测试仓库

##Intent

1. **最常见的：**

  > ```java
  > startActivity(new Intent(当前Act.this,要启动的Act.class));
  > ```
  
2. **通过Intent的ComponentName:**

  > ```java
  > ComponentName cn = new ComponentName("当前Act的全限定类名","启动Act的全限定类名");
  > Intent intent = new Intent();
  > intent.setComponent(cn);
  > startActivity(intent);
  > ```
  
3. **初始化Intent时指定包名：**
  
  > ```java
  > Intent intent = new Intent("android.intent.action.MAIN");
  > intent.setClassName("当前Act的全限定类名","启动Act的全限定类名");
  > startActivity(intent);
  > ```
