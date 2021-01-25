# **NIIT健康填报自动化**  
基于python，通过代码模拟运行打卡过程，实现一键自动化健康打卡，让我们美好的一天从早起打卡开始吧。

# **特别声明**  
- 本仓库发布的项目中涉及的任何脚本，仅用于测试和python学习研究，禁止用于任何商业用途,虚假上报等，请勿开展以此为目的的任何盈利和违法行为，违法必究！  
- 本脚本仅限无风险地区学生测试使用。
- 开发者对使用或不使用本脚本造成的问题不负任何责任，不对脚本执行效果做出任何担保，原则上不提供任何形式的技术支持。<code>tanglaoban</code> 保留随时更改或补充与删除项目的权利。  
**您一旦使用并复制了本仓库且本人制作的任何代码或项目，则视为<code>已接受</code>此声明，请仔细阅读**  

# **更新记录**  
邮箱通知功能，修改jktb.py文件对应参数
# **使用方法**  
**1.环境要求**
- 一个 24 小时开机的 Linux /windows操作系统（建议阿里云腾讯云学生机）
- Python 3.x以上，安装有 requests，Pyyaml 库  
 
**2.数据填写**  
- 打开config.yaml，填写学号，姓名，高德API KEY，cookie，x_csrf_token，当前所在地      
- 打开jktb.py ，填写个人识别码xxx，班级识别码yyy，学院识别码zzz  

**3.运行脚本**  
python3 jktb.py  

# **config.yaml 数据获取方法**  
1.进入<code> www.jiandaoyun.com</code>，选择企业成员登录自动进入，打开开发者工具（Chrome 可以使用 F12 快捷键），选中 Network 窗口：  

2.找到健康上报页面，点击上报，点击抓到的creta请求，将找到的cookie和x_csrf_toke存放在config.yaml 中  

3.在 Headers 下面找到 Form Data 这就是每次上报提交的信息参数。找到个人识别码_widget_1582448367786，班级识别码_widget_1582448368018，学院识别码_widget_1582699228446  
