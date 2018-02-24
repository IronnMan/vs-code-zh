# VS Code 交互式演练场
VS Code 功能非常齐全。 这个页面突出显示了它们中的一些，并且可以通过使用一些嵌入式编辑器来交互式地尝试它们。有关 VS Code 的编辑器功能的更多详细信息，请参阅我们的 [文档](https://code.visualstudio.com/docs#vscode).

- [Multi-cursor Editing](#multi-cursor-editing)（多光标编辑） - 块选择，选择所有的事件，添加额外的游标等等
- [IntelliSense](#intellisense) （智能感知）- 为您的代码和外部模块获取代码帮助和参数建议
- [Line Actions](#line-actions) （行动）- 快速移动线条来重新排序您的代码。
- [Rename Refactoring](#rename-refactoring) （重命名重构）- 快速重命名您的代码库中的符号。
- [Refactoring via Extraction](#refactoring-via-extraction) （通过提取进行重构）- 快速提取共同的代码到一个单独的函数或常量。
- [Formatting](#formatting)（格式化） - 使用内置的文档和选择格式让代码看起来很棒。
- [Code Folding](#code-folding)（代码折叠） - 通过折叠其他区域来关注代码中最相关的部分。
- [Errors and Warnings](#errors-and-warnings)（错误和警告） - 在输入时看到错误和警告。
- [Snippets](#snippets) （片段）- 花费更少的时间用片段打字。
- [Emmet](#emmet) - 集成的 Emmet 支持将 HTML 和 CSS 编辑提高到一个新的水平。
- [JavaScript Type Checking](#javascript-type-checking)（JavaScript类型检查） - 使用零配置的 TypeScript 对您的 JavaScript 文件执行类型检查。



## Multi-Cursor Editing
使用多个光标可以一次编辑文档的多个部分，从而大大提高您的工作效率。在下面的代码块中尝试以下操作：

1. 文本框选择 - 按 `Shift-Option-Cmd-Down`, `Shift-Option-Cmd-Right`, `Shift-Option-Cmd-Up`, `Shift-Option-Cmd-Left` 的任意组合选择一个文本块。用鼠标选择文字时，也可以按 `Shift+Option`。
2. 添加一个光标 - 按 `Option-Cmd-Up` 在上面添加一个新的光标，或者 `Option-Cmd-Down` 在下面添加一个新的光标。你也可以使用鼠标与 `Option+Click` 在任何地方添加光标。
3. 在所有出现的字符串上创建游标 - 选择一个字符串的一个实例，例如 `background-color` 并按下 `Shift-Cmd-L`。 现在你可以通过输入来替换所有的实例。

这是 Multi-Cursor Editing 的冰山一角。 查看选择菜单和我们的 [键盘快捷方式指南](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-macos.pdf) 以了解更多操作。

![keyboard Reference Guide](img/keyboard-guide.png)

> CSS Tipe: 你可能已经注意到，在上面的例子中，我们也为 CSS 提供了内嵌的颜色板，另外如果你把鼠标悬停在像 `#p1` 这样的元素上，我们将会展示如何用 HTML 表示。 这些色板也可以作为颜色选择器，让您轻松更改颜色值。 一些特定于语言的编辑器功能的简单示例。



## IntelliSense
Visual Studio Code 附带了强大的 IntelliSense for JavaScript and TypeScript 预安装。在下面的示例中，将文本光标放在错误下划线的前面，紧跟在点之后，按 `Control+Space` 来调用 IntelliSense。注意这个建议来自 Request API。

![intelli Sense](img/intelliSense.png)

> Tip: 当我们提供开箱即用的 JavaScript 和  TypeScript 支持时，其他语言可以通过许多 `extensions` 中的一个，通过更好的 IntelliSense 进行升级。



## Line Actions
由于处理整行文本非常常见，因此我们提供了一组有用的快捷方式来帮助解决这个问题。

1. 复制一行并分别用 `Shift-Option-Down` 或 `Shift-Option-Up` 将其插入当前位置的上方或下方。
2. 分别用 `Option+Up` 和 `Option+Down` 键向上或向下移动整行或者选择行。
3. 用 `Shift-Cmd-K` 删除整行。

![line Actions](img/lineActions.png)

> Tip: 另一个非常常见的任务是注释掉一段代码 - 你可以通过按下 `⌘/` 来切换注释。



## Rename Refactoring
重命名符号（如函数名称或变量名称）很容易。在字符 `Book` 前中点击，按 `F2` 来重命名所有实例 - 这将发生在项目中的所有文件中。你也可以在右键单击上下文菜单中看到重构。

![rename Refactoring](img/renameRefactoring.png)

> JSDoc Tip: 上面的例子还展示了另一种通过使用 `JSDoc` 注释来获得 IntelliSense 提示的方法。你也可以通过调用 `Book` 函数并在 IntelliSense 菜单中查看改功能的增强上下文以及参数来尝试此操作。



## Refactoring via Extraction
有时候你想把已经写好的代码重构成一个单独的函数或者常量，以后重用。选择你想重构的行并按下 `⌘.`，或者点击小灯泡，选择其中一个 `Extract to...` 选项。 通过选择第 3 行 的 `if` 语句中的代码或任何其他需要重构的常用代码来尝试。

![refactoring Via Extraction](img/refactoringViaExtraction.png)



## Formatting
如果没有一个好的格式化程序，保持你的代码整洁是很难的。幸运的是，用 `Shift-Option-F` 格式化整个文档的内容是很容易的。格式化可以通过 `右⌘K 左⌘F`应用于当前选择。 这两个选项也可以通过右键单击上下文菜单来获得。

![formatting](img/formatting.png)

> Tip: 其他格式化程序可以在 `extension gallery` 中找到。格式化支持也可以通过 `settings` 来配置，例如 启用 `editor.formatOnSave`。



## Code Folding
在大文件中，通常可以折叠代码段来提高可读性。要做到这一点，你可以简单地按 `Option-Cmd-[` 折叠代码，按 `Option-Cmd-]` 展开。折叠也可以通过左侧水槽中的 +/- 图标完成。要折叠所有部分，请使用 `⌘K ⌘0` 或展开全部使用 `K⌘ J⌘`。

![code Folding](img/codeFolding.png)

> Tip: 折叠是基于缩进，因此可以适用于所有语言。简单地缩进你的代码来创建一个可折叠的部分，你可以用 `⌘K ⌘1` 到 `⌘K ⌘5`这样的快捷折叠一定数量的关卡。



## Errors and Warnings
当你编辑代码时，错误或警告会以波浪线突出显示。在下面的示例中，你可以看到一些语法错误。 通过按 `F8`，你可以依次浏览它们并查看详细的错误信息。当你改正它们时，波形和滚动条指针将会更新。

![errors And Warnings](img/errorsAndWarnings.png)



## Snippets
通过使用片段，您可以大大加快编辑速度。只要输入 `try` 并从建议列表中选择 `trycatch` 并按下 `Tab` 来创建 `try`->`catch` 块。你的光标将放在文本 `error`，以便于编辑。如果存在多个参数，则按 `Tab` 跳转到改参数。

![snippets](img/snippets.png)

> Tip: `extension gallery` 包含几乎所有可以想象的框架和语言片段。你也可以创建自己的 `user-defined snippets`。



## Emmet
Emmet 将片段概念提升到了一个全新的高度：你可以键入类似 CSS 的表达式，这些表达式可以进行动态分析，并根据你输入的缩写产生输出。要使用 Emmet，只需要有效的 emmet 缩写或代码片段末尾用光标运行 `Emmet: Expand Abbreviation` 命令，即可进行扩展。

![emmet](img/emmet.png)

> Tip: [Emmet cheat sheet](https://docs.emmet.io/cheat-sheet/) 是 Emmet 语法建议的重要来源。要使用 `tab` 键来扩展 Emmet 缩写和代码片段，请使用 `emmet.triggerExpansionOnTab` 设置。



## JavaScript Type Checking
有时，检查 JavaScript 代码的类型可以帮助您发现可能没有发现的错误。你可以通过在你的文件顶部添加 `// @ts-check` 注释来针对你现有的 JavaScript 代码运行 TypeScript 类型检查器。

![javascript Type Checking](img/javascriptTypeChecking.png)

> Tip: 你还可以通过在工作区或用户设置中添加 `"javascript.implicitProjectConfig.checkJs": true` 来启用工作区或应用程序范围，并使用 `// @ts-nocheck` 和 `// @ts-ignore`。查看 [ VS Code 中的 JavaScript](https://code.visualstudio.com/docs/languages/javascript) 文档了解更多信息。




# Thanks!
那么，如果你已经走到这一步，那么你将有涉及到一些 Visual Studio Code 编辑功能。 但是现在请不要停止 :) 我们有许多 [其他文档](https://code.visualstudio.com/docs)，[介绍性视频](https://code.visualstudio.com/docs/getstarted/introvideos)以及产品的[提示和技巧](https://code.visualstudio.com/docs/getstarted/tips-and-tricks#vscode)，可以帮助你了解如何使用它。而你在这里的时候，还有一些你可以尝试的东西：

- 通过按 `` Control+` `` 打开集成终端，然后通过查看[终端文档](https://code.visualstudio.com/docs/editor/integrated-terminal)查看可能的内容
- 按 `Control-Shift-G` 进行版本控制。了解如何通过查看[版本控制文档](https://code.visualstudio.com/docs/editor/versioncontrol)来分阶段，提交，更改分支和查看差异等等
- 按 `Shift-Cmd-X` 浏览集成图库中的数千个扩展。改[文档](https://code.visualstudio.com/docs/editor/extension-gallery)将告诉你如何看到最流行的扩展，禁用已安装的扩展。

目前为止就这样了，

Happy Coding!






