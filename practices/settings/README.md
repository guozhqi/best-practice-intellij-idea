# IDE配置的基础知识
本篇主要了解一些IDEA的配置基础。

**[⬆ 回到頂端](#table-of-contents)**

------

## 目录
- 参考
- 配置的分类
- 配置的分层（作用域）


**[⬆ 回到頂端](#table-of-contents)**

------
## 参考
- [IEDA官方文档](https://www.jetbrains.com/help/idea/2024.1/working-with-projects.html#settings-types)


**[⬆ 回到頂端](#table-of-contents)**

------
## 配置的分类
IDEA中有三种类型的配置：
![xxxx](https://resources.jetbrains.com/help/img/idea/2024.1/settings-types.png)

- Module settings

    These settings apply only to one module and are stored in the .iml file. A module can have an SDK and a language level that are different from those configured for a project, and their own libraries. They can also carry a specific technology or a framework.

    For more information, refer to Module structure settings.
- Project settings

    These settings apply only to the current project. They are stored together with other project files in the .idea directory in the .xml format. For example, projects keep VCS settings, SDKs, code style and spellchecker settings, compiler output, libraries that are available for all modules within a project.

    For more information, refer to Project settings and Project structure settings.
- Global settings

    Global settings apply to all projects of a specific installation of IntelliJ IDEA. Such settings include IDE appearance (for example, themes and color schemes), the set of installed and enabled plugins, debugger settings, global inspection profiles, and much more.

    For more information, refer to IDE configuration.


**[⬆ 回到頂端](#table-of-contents)**

------
## 配置的分层（作用域）
IDEA 的设置项有2种不同的作用域，分为“全局-Global”和“项目级-Project”：
 - `Global`     
  全局设置适用于使用特定安装或版本的 IntelliJ IDEA 打开的所有项目。此类设置包括 IDE 外观（主题、配色方案、菜单和工具栏）、通知设置、已安装和启用的插件集、调试器设置、代码完成等。全局设置存储在配置目录中。
-  `Project`    
  项目设置仅适用于当前项目，除非将其配置为新项目的默认设置。此类设置包括 VCS 配置、代码样式选项、语言检查列表等

#### 如何配置

- 在工程界面，依次点击 "File" -> "Settings..." 进入设置页面；

  或者直接通过快捷键 “ctrl + alt + s" 进入设置页面；

  ![open-setting-panel-from-project](https://picgo-daily.oss-cn-guangzhou.aliyuncs.com/picgo-daily/2023/d1b03e77e437778b3db2a39bbd5da83f.png)


### 区分全局配置和项目级配置
以上两种方式都能进入IDEA的配置Dialog去，只是入口不同罢了，那我们如何区分全局配置和项目级配置呢？
答案： 通过配置项的图标来区分。
全局配置和项目级配置是通过配置项边上的小图标来区分的，![xxx](https://resources.jetbrains.com/help/img/idea/2024.1/app.general.projectConfigurable.svg)，也就是说在项目中打开setting后我们配置一些不带图标的配置项，它改变的也是全局配置，所有的项目都会生效（已验证）

![xxx](https://resources.jetbrains.com/help/img/idea/2024.1/ide-settings-preferences.png)


设置对话框中看到一个设置项旁边有“当前项目”的图标的，说明该设置项只对当前工程生效。其余的是全局配置，对所有工程都生效。

### 澄清：它不是全局配置
- 在 IDEA 欢迎页面，点击 ”Customize" -> "All settings..." 进入设置界面：

  ![open-settings-panel-from-welcome](https://picgo-daily.oss-cn-guangzhou.aliyuncs.com/picgo-daily/2023/3065ccac37c461310f291d527172a36d.png)

  PS: 以上两种方式都能进入IDEA的配置Dialog去，只是入口不同罢了,从这边进来并不代表全局配置。

**[⬆ 回到頂端](#table-of-contents)**

------
## 总结
了解配置的第一步，配置分层分类


  **[⬆ 回到頂端](#table-of-contents)**

------









