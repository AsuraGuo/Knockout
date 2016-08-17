# Knockout
# 实习的公司在用这个框架就简单的学习一下
# Knockout是一个轻量级的UI类库，通过应用MVVM模式使JavaScript前端UI简单化。
# Knockout有如下4大重要概念：
#    声明式绑定 (Declarative Bindings)：使用简明易读的语法很容易地将模型(model)数据关联到DOM元素上。
#    UI界面自动刷新 (Automatic UI Refresh)：当您的模型状态(model state)改变时，您的UI界面将自动更新。
#    依赖跟踪 (Dependency Tracking)：为转变和联合数据，在你的模型数据之间隐式建立关系。
#    模板 (Templating)：为您的模型数据快速编写复杂的可嵌套的UI。

# Knockout是一个以数据模型（data model）为基础的能够帮助你创建富文本，响应显示和编辑用户界面的JavaScript类库。
# 任何时候如果你的UI需要自动更新（比如：更新依赖于用户的行为或者外部数据源的改变），KO能够很简单的帮你实现并且很容易维护。

# 重要特性:
#    优雅的依赖追踪- 不管任何时候你的数据模型更新，都会自动更新相应的内容。
#    声明式绑定- 浅显易懂的方式将你的用户界面指定部分关联到你的数据模型上。
#    灵活全面的模板- 使用嵌套模板可以构建复杂的动态界面。
#    轻易可扩展- 几行代码就可以实现自定义行为作为新的声明式绑定。
# 额外的好处：
#    纯JavaScript类库 – 兼容任何服务器端和客户端技术
#    可添加到Web程序最上部 – 不需要大的架构改变
#    简洁的 – Gzip之前大约25kb
#    兼容任何主流浏览器 (IE 6+、Firefox 2+、Chrome、Safari、其它)
#    Comprehensive suite of specifications （采用行为驱动开发） - 意味着在新的浏览器和平台上可以很容易通过验证。
# 开发人员如果用过Silverlight或者WPF可能会知道KO是MVVM模式的一个例子。
# 如果熟悉 Ruby on Rails 或其它MVC技术可能会发现它是一个带有声明式语法的MVC实时form。
# 换句话说，你可以把KO当成通过编辑JSON数据来制作UI用户界面的一种方式… 不管它为你做什么


# MVVM模式和view model的概念。
# Model-View-View Model (MVVM) 是一种创建用户界面的设计模式。 描述的是如何将复杂的UI用户界面分成3个部分：
# model: 你程序里存储的数据。这个数据包括对象和业务操作（例如：银子账户可以完成转账功能）， 并且独立于任何UI。
#     使用KO的时候，通常说是向服务器调用Ajax读写这个存储的模型数据。
# view model: 在UI上，纯code描述的数据以及操作。
#     例如，如果你实现列表编辑，你的view model应该是一个包含列表项items的对象和暴露的add/remove列表项（item）的操作方法。
# 　　　　
#     注意这不是UI本身：它不包含任何按钮的概念或者显示风格。它也不是持续数据模型 – 包含用户正在使用的未保存数据。
#     使用KO的时候，你的view models是不包含任何HTML知识的纯JavaScript 对象。
#     保持view model抽象可以保持简单，以便你能管理更复杂的行为。
# 
# view: 一个可见的，交互式的，表示view model状态的UI。
#     从view model显示数据，发送命令到view model（例如：当用户click按钮的时候） ，任何view model状态改变的时候更新。
# 使用KO的时候，你的view就是你带有绑定信息的HTML文档，这些声明式的绑定管理到你的view model上。
# 或者你可以使用模板从你的view model获取数据生成HTML。
