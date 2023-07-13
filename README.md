## mini-AGI 迷你AGI
https://github.com/ziwang-com/mini-AGI

简单实用的一站式AGI架构，内置原生矢量数据库，支持本地化LLM模型，agent，智能链chain，prompt提示词

10行代码，即可复刻经典GPT开源项目：localGPT，privateGPT。

单一py源码模块文件，实现langchain+prompt提示词+llm+矢量数据库+AGI(autoGPT,babyAGI) 80%功能。

<img width="271" alt="mini-agi-logo" src="https://github.com/ziwang-com/miniAGI/assets/11691791/b1f9f547-205c-4c17-8f21-3ff834874ef0">

mini-AGI是zw-AGI的免费开源版本，删除了部分商务模块。

https://github.com/ziwang-com/zwAGI

## 【已完成功能】
* 10行代码，即可即复刻经典GPT开源项目：localGPT，privateGPT，
* 单一py源码模块文件，实现langchain+prompt提示词+llm+矢量数据库+AGI(autoGPT,babyAGI) 80%功能。
* 单文件模块源码，copy工作目录，直接import，无需安装。
* 内置式原生矢量数据库，基于pandas，生态完整。
* 支持：txt，csv，docx, ppt，pdf，markdown等，多种格式文件数据导入。
* 开放式prompts提示词文档，内置多组常用prompts提示词。
* 内置式llm调用：
  * 支持清华cgatGLM-6B二代模型，毕竟是国内最强开源llm大模型。
  * 首批支持ggml格式，llamcpp纯cpu调用，zw-vicuna-7B，13B，33B实测通过。
  * 支持大部分主流开源模型，包括：LLaMA 🦙、Alpaca、 GPT4All、 Chinese LLaMA / Alpaca、 Vigogne (French)、 Vicuna、 GGML、Koala、 OpenBuddy 🐶 (Multilingual)、 Pygmalion  / MetharmeB、 WizardLM、 Baichuan and its derivations (such as baichuan-sft)

## 【todo-list，计划完成功能】
* agent代理
* tool工具应用
* 智能链chain
* 开放式免费web搜索，免密匙
* 。。。。。。



## 【mini-agi模块库文件说明】
* 迷你AGI结构很简单，单一python文件结构。保存在mini-xlib目录当中。
* 大部分结构，代码，都是原创，强调工程实用性，约定优先。
* 部分代码，参考了相关开源项目，在此表示感谢。

## 【core核心文件说明】
* mini_agi.py，模块库核心文件
* prompt.yaml，提示词模板，字典格式，采用yaml文件保存，用户可以自己添加。

## 【plungin插件说明】
迷你AGI插件，也是采用单一py文件模式，简单明了。
发布时，内置了3个插件案例源码，方便大家扩展。

* mini_glm.py，清华chatGLM2-6B插件，支持国产llm项目。
* mini_gpt.py，openAI-api接口插件，使用前自己在源码文件设置好网址，key密匙
* mini_llm.py，ggml模型插件，支持zw-vicuan-7B/13B/33B中文汉化版，实测通过。
* 安装llama-cpp-python模块库，需要c语言编译器。
* 	具体细节参看：
https://github.com/ggerganov/llama.cpp
https://github.com/abetlen/llama-cpp-python
	

## 【QA查询demo示例程序】
* tur001-qa.py，不到10行代码，完美复刻经典GPT开源项目：localGPT，privateGPT。
* tur002-gpt.py，GPT3.5-api接口模式

* tur03-llm.py，ggml模型文件调用，支持zw-vicuan-7B/13B/33B中文汉化版，实测通过。


## 【VDB数据库生成demo示例程序】
VDB矢量数据库，采用标准pandas DataFrame格式。
数据库文件扩展名是pkl，存储采用的是feather格式。

* tur011_db8fn.py，从csv文件生成vec矢量数据库
* tur012_db8dir.py，从目录批量生成vec矢量数据库，支持子目录结构，支持多种文件格式，示例程序demo包括：doc，txt，pdf等多种格式

## 【models模型文件说明】
默认模型保存在libs目录下，

* libs\all-MiniLM-L6-v2，文本矢量转换模型
* libs\zw-v7cn.bin，智王zw-vicuna-13B-cn中文汉化版
* libs\zw-v33cn.bin，智王zw-vicuna-33B-cn中文汉化版
* libs\chatglm2-6b，清华ChatGLM2-6B模型

以上模型，可以在智王百度网盘下载，也可以自己在huggingface等网站下载。
## 【智王AI资源库】百度网盘提取码：hiks 
https://pan.baidu.com/s/1EH19ablXVLYQP1f-IaPS-Q?pwd=hiks
如有更改，最新下载地址请参见: QQ群文件：655402626（GPT+千人QQ大群）


## 【mini-agi迷你AGI懒人包】
为方便大家使用，稍后会推出【mini-agi迷你AGI懒人包】。
集成了zw-GPT-studio智王GPT集成式python开发平台，基本模型库，解压即用。
windows平台，需安装好cuda12.x运行环境。
linux、mac-os，请用vbox等虚拟机模式加载。

  <img width="702" alt="gptx-3x1" src="https://github.com/ziwang-com/miniAGI/assets/11691791/1ac6ffbe-5b93-436c-9a4d-f54a02e6b62c">

## 【欢迎加盟】
赠人玫瑰，手有余香。

欢迎各位网友，加盟mini-AGI开源项目组。

有意者请扫描上图右侧: zw群主-微信二维码.


