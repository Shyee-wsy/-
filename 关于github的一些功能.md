# Issues    
### 一、issue 是什么？  
Issue 是指一项待完成的工作，通常与系统的改进相关，中文可以翻译成“问题”或“事务”。  
### 二、github Issue的功能  
#### 1. 基本用法  
```
1. 进入Issue面板，点击“New Issue”按钮，新建一个Issue；
2. 左侧填入Issue的标题和内容，右侧是四个配置项（只有项目管理者才能看见）
- Assignees:人员  
- Labels: 标签  
- Projects: 项目
- MileStone: 里程碑  
3. 想要查看和操作所有与自己相关的Issue，访问首页的Issue，即可打开Issue全局视图。
- Created: 你创建的 Issue；
- Assigned: 分配给你的Issue；
- Mentioned: 提及你的Issue；（别人在Issue里面@了你）  
4. Issue详情页的最下面：Transfer issue ，可以将该Issue转移到其他仓库，转移之后该仓库的Issue将不存在。
```  
##### 下面介绍四个配置项  
<blockquote>1.1 Assignee</blockquote>   
 Assignee 选择框用于从当前仓库的所有成员之中，指派某个Issue的处理人员。  
<blockquote>1.2 Label </blockquote>  
 Issue 可以贴上标签，这样有利于分类管理和过滤查看。可以选择默认列表里面的标签，也可以添加自定义标签。  
<blockquote>1.3 Milestone </blockquote> 
 里程碑，用作Issue的容器，相关的Issue可以放在一个Milestone 里面。常见的例子是不同版本和迭代，都可以做成milestone.    
 参考：https://help.github.com/en/articles/about-issues   
 http://www.ruanyifeng.com/blog/2017/08/issue.html 
 
# project boards  
### 一、看板是什么？  
将所有需要完成的任务做成卡片，贴在一块白板上面，清晰的看见项目的进度管理，这就是看板。你可以根据实际情况，或者项目的开发进度，将项目周期（看板模块的title）
设置成Todo，Doing，Done等等。或者更多的列。  
### 二、github的看板功能  
#### 1. 基本用法  
```
1.在仓库首页进入 Projects面板；  
2.点击“Create a project”，新建一个Project，接着点击“Add a column”按钮，为项目新建若干个列，列可拖动。每个列中可新建notes，notes可添加至Issue中。
```     
# Wiki  
### 一、Wiki是什么？    
wiki是一种协作的写作模式，来源于夏威夷语，它最大的特点就是分享性，开放性以及互动性。wiki站点允许任何访问它的用户都可以修改、编辑以及创建上面的内容。 
wiki软件，是一种运行在php+mysql运行环境的百科系统软件。用wiki软件可以迅速地搭建起一个wiki网站。国内目前使用最普遍的wiki软件有HDwiki(互动中文wiki系统)以及mediawiki。 
两者各有特点。HDwiki，是中国第一家拥有自主知识产权的中文wiki系统，适用于国内wiki爱好者； 
mediawiki是世界上使用最多的wiki系统，在世界范围内使用比较广泛。  

### 二、Github的Wiki是什么？    
每个 GitHub 仓库都有一个托管文档的部分，称为 wiki。 您可以使用仓库的 wiki 共享项目的长内容，例如如何使用项目，您是如何设计项目的，或者其核心原则是什么。 自述文件快速介绍项目的内容，而您可以使用 wiki 提供其他文档。
Wikis 可在公共仓库中公开，也可在私有仓库中限于对仓库具有访问权限的人访问。  
您可以直接在 GitHub 上编辑 wikis，也可在本地编辑 wiki 文件。 默认情况下，只有能够写入仓库的人才可更改 wikis，但您可以允许 GitHub 上的每个人参与公共仓库中的 wiki。  
参考地址：
https://blog.csdn.net/xiyangyang8110/article/details/53140310  
https://help.github.com/cn/articles/about-wikis  
  
# Github的Security   
```
Github的Security主要包括三个部分:  
- Alerts ()
- Advisories (通告)
- Policy (政策)
```  
### Policy（安全政策）  
#### 关于安全政策  
为了让人们了解如何负责任地报告您的仓库中存在的安全漏洞，您可以将 SECURITY.md 文件添加到仓库的根文件夹 docs 或 .github。 当有人在您的仓库中创建议题时，就会看到项目安全政策的链接。  
#### 添加安全政策到仓库  
```
1. 在 GitHub 上，导航到仓库的主页面。  
2. 在仓库名称下，单击 Security（安全）。 
3. 在左侧边栏中，单击 Policy（政策）。  
4. 单击 Start setup（开始设置）。  
5. 在新的 SECURITY.md 文件中，添加关于项目受支持版本以及如何报告漏洞的信息。
6. 在页面底部，键入简短、有意义的提交消息，描述您对文件所做的更改。您可以在提交消息中将提交归因于多个作者。
7. 在 commit message（提交消息）字段下方，单击 email address（电子邮件地址）下拉菜单，然后选择 Git 作者电子邮件地址。此下拉菜单中只显示经验证电子邮件地址。 如果启用了电子邮件地址保密，则 <username>@users.noreply.github.com 为默认的提交作者电子邮件地址。
8. 在 commit message（提交消息）字段下方，决定要将提交添加到当前分支还是添加到新分支。如果当前分支为 master，则应选择为提交创建新分支，然后创建拉取请求。
9. 单击 Propose file change（提议文件更改）。
```
### Advisories(通告)  
#### 关于维护员安全员通告  
1. 您可以使用维护员安全通告来私下讨论、修复和发布有关仓库中安全漏洞的信息。  
2. 创建通告草稿，并使用草稿私下讨论漏洞对项目的影响  
3. 私下协作在临时私有复刻中修复漏洞  
4. 发布通告向社区提醒漏洞  
5. GitHub 将审查每一个发布的通告，并且可能使用通告向受影响的仓库发送安全警报。  
#### 创建维护员安全通告  
您可以创建通告草稿，以私下讨论和修复开源项目中的安全漏洞。  
任何对仓库有管理员权限的人都可以创建安全通告。
```
1.在左侧边栏中，单击 Advisories（通告）。
2.单击 New draft advisory（新建通告草稿）
3.键入安全通告的标题。
4.键入安全漏洞的说明。
5.单击 Create draft advisory（创建通告草稿）。
```
#### 添加协作者到维护员安全通告  
您可以添加其他用户或团队与您协作处理安全通告。  
```
在页面右侧的 "Access and visibility"（访问和可见性）下，输入要添加到仓库的用户或团队名称。
```



参考：https://help.github.com/cn/articles/adding-a-security-policy-to-your-repository  
https://help.github.com/cn/articles/managing-security-vulnerabilities-in-your-project
