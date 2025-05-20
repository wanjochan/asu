
# Python 编程基础

## 1. Python 安装与环境配置
- **下载与安装**：
  - 从官网 [www.python.org](http://www.python.org) 下载 Python，推荐使用 3.6 或以上版本（如 3.7、3.9）。
  - 安装时勾选“添加到系统路径”，方便在命令行运行。
- **自带工具**：
  - 安装完成后自动包含 IDLE，一个简单的 Python 开发环境。

## 2. 开发环境选择
- **IDLE**：Python 自带，适合初学者，功能简单。
- **Visual Studio**：支持 Python，提供强大功能，适合多语言开发。
- **PyCharm**：专为 Python 设计的 IDE，功能丰富。
- **VSCode**：轻量级，支持 Python 插件，跨平台使用。

## 3. Python 基本语法
- **输出**：`print("Hello world")` 用于打印。
- **变量**：动态类型，无需声明类型，例如 `i = 5` 或 `j = "hello world"`。
- **缩进**：使用 Tab 或空格（需统一）定义代码块，严格对齐。

## 4. 函数定义与调用
- **定义函数**：  
  ```python
  def 函数名(参数):
      代码块
  ```
- **调用**：`函数名(参数)`。
- **全局变量**：函数外定义，可在函数内访问或修改（需用 `global` 关键字）。
- **局部变量**：函数内定义，仅函数内有效。
- **示例**：
  ```python
  i = 5  # 全局变量
  def foo(n):
      global i
      i += 4
      print("in foo i =", i)
  def main():
      foo(10)
      print("in main i =", i)
  main()
  ```

## 5. 控制流语句
- **if 语句**：
  ```python
  if 条件:
      代码块
  elif 条件:
      代码块
  else:
      代码块
  ```
- **while 循环**：
  ```python
  while 条件:
      代码块
  ```
- **for 循环**（类似 Foreach）：
  ```python
  for 变量 in 集合:
      代码块
  ```
- **注意**：无 `do while`，`for` 用于整数循环，`foreach` 用于集合遍历。

## 6. 列表操作
- **定义**：`列表名 = [元素1, 元素2, ...]`。
- **长度**：`len(列表名)`。
- **遍历**：`for 元素 in 列表: 代码块`。
- **示例**：计算平均值
  ```python
  def averageofList(num):
      sum = 0
      for t in num:
          sum += t
      return sum / len(num)
  print(averageofList([19, 21, 46, 11, 18]))  # 输出 23.0
  ```

## 7. 库的使用
- **导入**：`import 库名`。
- **调用**：`库名.函数名(参数)`。
- **示例**：使用 `statistics` 库
  ```python
  import statistics
  data = [11, 21, 11, 19, 46, 21, 19, 29, 21, 18, 3, 11, 11]
  print("mean =", statistics.mean(data))
  print("median =", statistics.median(data))
  print("mode =", statistics.mode(data))
  print("stdev =", statistics.stdev(data))
  print("variance =", statistics.variance(data))
  ```

## 8. 文件操作
- **打开文件**：`with open("文件名") as f:`。
- **读取**：`f.readlines()` 获取所有行。
- **关闭**：`with` 语句自动关闭，或手动 `f.close()`。
- **示例**：读取文件并计算平均值
  ```python
  sum = 0
  n = 0
  with open('mydata.txt') as f:
      data = f.readlines()
      for d in data:
          if d:
              sum += int(d)
              n += 1
  print(sum / n)
  ```

这份内容精华简明扼要，涵盖了 Python 编程的核心基础，适合快速复习和备考使用。你可以通过反复阅读和运行示例代码加深理解。


# Python 编程基础内容精华

## 1. Python 安装与环境配置
- **下载与安装**：
  - 从官网 [www.python.org](http://www.python.org) 下载 Python，推荐使用 3.6 或以上版本（如 3.7、3.9）。
  - 安装时勾选“添加到系统路径”，方便在命令行运行。
- **自带工具**：
  - 安装完成后自动包含 IDLE，一个简单的 Python 开发环境。

## 2. 开发环境选择
- **IDLE**：Python 自带，适合初学者，功能简单。
- **Visual Studio**：支持 Python，提供强大功能，适合多语言开发。
- **PyCharm**：专为 Python 设计的 IDE，功能丰富。
- **VSCode**：轻量级，支持 Python 插件，跨平台使用。

## 3. Python 基本语法
- **输出**：`print("Hello world")` 用于打印。
- **变量**：动态类型，无需声明类型，例如 `i = 5` 或 `j = "hello world"`。
- **缩进**：使用 Tab 或空格（需统一）定义代码块，严格对齐。

## 4. 函数定义与调用
- **定义函数**：  
  ```python
  def 函数名(参数):
      代码块
  ```
- **调用**：`函数名(参数)`。
- **全局变量**：函数外定义，可在函数内访问或修改（需用 `global` 关键字）。
- **局部变量**：函数内定义，仅函数内有效。
- **示例**：
  ```python
  i = 5  # 全局变量
  def foo(n):
      global i
      i += 4
      print("in foo i =", i)
  def main():
      foo(10)
      print("in main i =", i)
  main()
  ```

## 5. 控制流语句
- **if 语句**：
  ```python
  if 条件:
      代码块
  elif 条件:
      代码块
  else:
      代码块
  ```
- **while 循环**：
  ```python
  while 条件:
      代码块
  ```
- **for 循环**（类似 Foreach）：
  ```python
  for 变量 in 集合:
      代码块
  ```
- **注意**：无 `do while`，`for` 用于整数循环，`foreach` 用于集合遍历。

## 6. 列表操作
- **定义**：`列表名 = [元素1, 元素2, ...]`。
- **长度**：`len(列表名)`。
- **遍历**：`for 元素 in 列表: 代码块`。
- **示例**：计算平均值
  ```python
  def averageofList(num):
      sum = 0
      for t in num:
          sum += t
      return sum / len(num)
  print(averageofList([19, 21, 46, 11, 18]))  # 输出 23.0
  ```

## 7. 库的使用
- **导入**：`import 库名`。
- **调用**：`库名.函数名(参数)`。
- **示例**：使用 `statistics` 库
  ```python
  import statistics
  data = [11, 21, 11, 19, 46, 21, 19, 29, 21, 18, 3, 11, 11]
  print("mean =", statistics.mean(data))
  print("median =", statistics.median(data))
  print("mode =", statistics.mode(data))
  print("stdev =", statistics.stdev(data))
  print("variance =", statistics.variance(data))
  ```

## 8. 文件操作
- **打开文件**：`with open("文件名") as f:`。
- **读取**：`f.readlines()` 获取所有行。
- **关闭**：`with` 语句自动关闭，或手动 `f.close()`。
- **示例**：读取文件并计算平均值
  ```python
  sum = 0
  n = 0
  with open('mydata.txt') as f:
      data = f.readlines()
      for d in data:
          if d:
              sum += int(d)
              n += 1
  print(sum / n)
  ```
