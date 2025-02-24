---
Order: 5
Area: copilot
TOCTitle: Code Completions
ContentId: 7ab2cd6c-45fd-4278-a6e8-1c9e060593ea
PageTitle: AI-powered code completions with GitHub Copilot
DateApproved: 10/29/2024
MetaDescription: Enhance your coding with AI-powered code completions from GitHub Copilot in Visual Studio Code.
MetaSocialImage: images/shared/github-copilot-social.png
---
# Code completions with GitHub Copilot in VS Code

GitHub Copilot acts as an AI-powered pair programmer, automatically offering suggestions to complete your code, comments, tests, and more. It provides these suggestions directly in the editor while you write your code, and it can work with a broad range of programming languages and frameworks.

## Getting started

1. Install the GitHub Copilot extension. This also installs the GitHub Copilot Chat extension.

    > <a class="install-extension-btn" href="vscode:extension/GitHub.copilot">Install the GitHub Copilot extension</a>

1. Follow the steps in the [Copilot setup guide](/docs/copilot/setup.md) to configure GitHub Copilot in VS Code.

    > [!TIP]
    > If you don't yet have a GitHub Copilot subscription, sign up for a [GitHub Copilot free trial](https://github.com/login?return_to=%2fgithub-copilot%2fsignup) in your personal account.

1. Get going with these hands-on tutorials to learn how to use GitHub Copilot in VS Code.

    * [GitHub Copilot Quickstart](/docs/copilot/getting-started.md) - discover the key features of GitHub Copilot in VS Code.

    * [Copilot Chat Tutorial](/docs/copilot/getting-started-chat.md) - get started with AI chat conversations.

## Inline suggestions

Copilot offers code suggestions as you type: sometimes the completion of the current line, sometimes a whole new block of code. You can accept all, or part of a suggestion, or you can keep typing and ignore the suggestions.

Notice in the following example how Copilot suggests an implementation of the `calculateDaysBetweenDates` JavaScript function by using dimmed *ghost text*:

![JavaScript ghost text suggestion.](images/inline-suggestions/js-suggest.png)

When you're presented with an inline suggestion, you can accept it with the `kbstyle(Tab)` key.

Copilot tries to apply the same coding style for the code suggestions that you already have in your code. Notice in the following example that Copilot applies the same input parameter naming scheme from the `add` method for the suggested `subtract` method.

![JavaScript ghost text suggestion.](images/inline-suggestions/ts-suggest-parameter-names.png)

### Partially accepting suggestions

You might not want to accept an entire suggestion from GitHub Copilot. You can use the `kb(editor.action.inlineSuggest.acceptNextWord)` keyboard shortcut to accept either the next word of a suggestion, or the next line.

### Alternative suggestions

For any given input, Copilot might offer multiple, alternative suggestions. You can hover over the suggestion to any of the other suggestions.

![Hovering over inline suggestions enables you to select from multiple suggestions](images/inline-suggestions/copilot-hover-highlight.png)

### Generate suggestions from code comments

Instead of relying on Copilot to provide suggestions, you can provide hints about what code you expect by using code comments. For example, you could specify a type of algorithm or concept to use (for example, "use recursion" or "use a singleton pattern"), or which methods and properties to add to a class.

The following example shows how to instruct Copilot to create a class in TypeScript to represent a student, providing information about methods and properties:

![Use code comments to let Copilot generate a Student class in TypeScript with properties and methods.](images/inline-suggestions/ts-suggest-code-comment.png)

## Enable or disable inline suggestions

You can temporarily enable or disable code completions either for all languages, or for specific languages only.

1. The GitHub Copilot status icon in the VS Code Status Bar indicates whether GitHub Copilot is enabled or disabled.

    ![Screenshot showing the VS Code status bar, highlighting the Copilot icon that indicates Copilot is active.](./images/inline-suggestions/vscode-status-bar-copilot-active.jpg)

1. To enable or disable Copilot completions, first select the GitHub Copilot icon in the Status Bar.

1. If you are disabling GitHub Copilot, you are asked whether you want to disable suggestions globally, or for the language of the file you are currently editing.

    * To disable suggestions from GitHub Copilot globally, select **Disable Globally**.
    * To disable suggestions from GitHub Copilot for the specified language, select **Disable for \<language\>**.

    ![Screenshot showing the VS Code command menu for Copilot, highlighting the options to disable completions.](./images/inline-suggestions/copilot-disable-completions.png)

## Tips & tricks

### Context

To give you relevant inline suggestions, Copilot looks at the current and open files in your editor to analyze the context and create appropriate suggestions. Having related files open in VS Code while using Copilot helps set this context and lets the Copilot see a bigger picture of your project.

### Settings

* `setting(editor.inlineSuggest.enabled)` - enable or disable inline completions.

* `setting(editor.inlineSuggest.fontFamily)` - configure the font for the inline completions.

* `setting(editor.inlineSuggest.showToolbar)` - enable or disable the toolbar that appears for inline completions.

* `setting(editor.inlineSuggest.syntaxHighlightingEnabled)` - enable or disable syntax highlighting for inline completions.

## Next steps

* Get started with the introductory [Copilot tutorial](/docs/copilot/getting-started-chat.md) to get set up with Copilot in VS Code and experience Copilot hands-on.

* Learn how you can use AI chat conversations with [Copilot Chat](/docs/copilot/copilot-chat.md).

## Additional resources

You can read more about [Copilot](https://github.com/features/copilot) and how to use it in VS Code in the [GitHub Copilot documentation](https://docs.github.com/copilot/getting-started-with-github-copilot?tool=vscode).

Or check out the [VS Code Copilot Series](https://www.youtube.com/playlist?list=PLj6YeMhvp2S5_hvBl2SE-7YCHYlLQ0bPt) on YouTube, where you can find more introductory content and programming-specific videos for using Copilot with [Python](https://www.youtube.com/watch?v=DSHfHT5qnGc), [C#](https://www.youtube.com/watch?v=VsUQlSyQn1E), [Java](https://www.youtube.com/watch?v=zhCB95cE0HY), [PowerShell](https://www.youtube.com/watch?v=EwtRzAFiXEM), [C++](https://www.youtube.com/watch?v=ZfT2CXY5-Dc), and more.
