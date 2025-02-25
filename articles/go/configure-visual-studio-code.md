---
title: Configure Visual Studio Code for Go development
description: This article helps you configure Visual Studio Code for Go development.
ms.date: 11/11/2021
ms.topic: quickstart
ms.custom: devx-track-go
---

# Configure Visual Studio Code for Go development

In this quickstart, you'll install and configure the [Go for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=golang.Go) extension.

In the [Go Developer Survey 2020 Results](https://go.dev/blog/survey2020-results), **41%** of respondents chose Visual Studio Code as their *most preferred editor* for Go. This makes Visual Studio Code the most popular editor for Go developers.

Visual Studio Code and the Go extension provide IntelliSense, code navigation, and advanced debugging. In this quickstart, you'll configure Visual Studio Code. Then you'll write, run, and debug a sample Go program.

![A screenshot showing a Go program within Visual Studio Code](./media/configure-visual-studio-code/visual-studio-code.png)

<!-- retake screenshot, dir name is sample-app now -->

## 1. Install Go

Follow these steps to install Go:

1. In a web browser, go to [golang.org/doc/install](https://golang.org/doc/install).
1. Download the version for your operating system.
1. Once downloaded, run the installer.
1. Open a command prompt, then run `go version` to confirm Go was installed.

## 2. Install Visual Studio Code

Follow these steps to install Visual Studio Code:

1. In a web browser, go to [code.visualstudio.com](https://code.visualstudio.com/).
1. Download the version for your operating system, supports Windows, Linux, and macOS.
1. Once downloaded, run the installer. This will only take a minute.

## 3. Install the Go extension

| Instructions    | Screenshot |
|:----------------|-----------:|
| In Visual Studio Code, bring up the Extensions view by clicking on the Extensions icon in the Activity Bar. Or use keyboard shortcut (Ctrl+Shift+X). | :::image type="content" source="./media/configure-visual-studio-code/search-extensions-240px.png" alt-text="A screenshot showing how search for the Go extension." lightbox="./media/configure-visual-studio-code/search-extensions.png"::: |
| Search for the Go extension, then select install. | :::image type="content" source="./media/configure-visual-studio-code/install-go-extension-240px.png" alt-text="A screenshot showing how to use the search box in the top tool bar to find App Services in Azure." lightbox="./media/configure-visual-studio-code/install-go-extension.png"::: |

## 4. Update the Go tools

| Instructions    | Screenshot |
|:----------------|-----------:|
| In Visual Studio Code, open **Command Palette**'s **Help** > **Show All Commands**. Or use the keyboard shortcut (Ctrl+Shift+P) | :::image type="content" source="./media/configure-visual-studio-code/search-extensions-240px.png" alt-text="A screenshot showing how search the Command Palette." lightbox="./media/configure-visual-studio-code/search-extensions.png"::: |
| Search for `Go: Install/Update tools` then run the command from the pallet | :::image type="content" source="./media/configure-visual-studio-code/install-go-tools-240px.png" alt-text="A screenshot showing how to run the Go: install/update tool from the command pallet." lightbox="./media/configure-visual-studio-code/install-go-tools.png"::: |
| When prompted, select all the available Go tools then click OK.  | :::image type="content" source="./media/configure-visual-studio-code/select-all-go-tools-240px.png" alt-text="A screenshot showing how to update all the available Go tools." lightbox="./media/configure-visual-studio-code/select-all-go-tools.png"::: |
| Wait for the Go tools to finish updating.  | :::image type="content" source="./media/configure-visual-studio-code/go-tools-install-240x.png" alt-text="A screenshot showing all the Go tools that were updated." lightbox="./media/configure-visual-studio-code/go-tools-install.png"::: |

## 5. Write a sample Go program

| Instructions    | Screenshot |
|:----------------|-----------:|
| In Visual Studio Code, open the folder where you'll create the root directory of your Go application. To open the folder, click the Explorer icon in the Activity Bar then click **Open Folder**. | :::image type="content" source="./media/configure-visual-studio-code/open-folder-240px.png" alt-text="A screenshot showing how to create a new folder." lightbox="./media/configure-visual-studio-code/open-folder.png"::: |
| Click **New Folder** in the Explorer panel, then Create the root director for your sample Go application named `sample-app` | :::image type="content" source="./media/configure-visual-studio-code/create-folder-240px.png" alt-text="A screenshot showing how to create a folder in vs code." lightbox="./media/configure-visual-studio-code/create-folder.png"::: |
| Click **New File** in the Explorer panel, then name the file `main.go` | :::image type="content" source="./media/configure-visual-studio-code/create-file-240px.png" alt-text="A screenshot showing how to create a file in vs code." lightbox="./media/configure-visual-studio-code/create-file.png"::: |
| Open a terminal, **Terminal > New Terminal**, then run the command `go mod init sample-app` to initialize your sample Go app.   | :::image type="content" source="./media/configure-visual-studio-code/run-go-mod-240px.png" alt-text="A screenshot running the go mod init command." lightbox="./media/configure-visual-studio-code/run-go-mod.png"::: |
| Copy the following code into the `main.go` file.   | :::image type="content" source="./media/configure-visual-studio-code/visual-studio-code-240px.png" alt-text="A screenshot displaying a sample Go program." lightbox="./media/configure-visual-studio-code/visual-studio-code.png"::: |

Sample code:

```go
package main

import "fmt"

func main() {
    name := "Go Developers"
    fmt.Println("Azure for", name)
}
```

## 6. Run the debugger

| Instructions    | Screenshot |
|:----------------|-----------:|
| Create a break point on line 7 by left clicking to the left of the numbered line. Or place your cursor on line 7 and hit F9. | :::image type="content" source="./media/configure-visual-studio-code/create-breakpoint-240px.png" alt-text="A screenshot showing how to set a breakpoint." lightbox="./media/configure-visual-studio-code/create-breakpoint.png"::: |
| Bring up the Debug view by clicking on the debug icon in the Activity Bar on the side of Visual Studio Code. Or use keyboard shortcut (Ctrl+Shift+D). | :::image type="content" source="./media/configure-visual-studio-code/run-debugger-240px.png" alt-text="A screenshot showing how to navigate to the debug panel." lightbox="./media/configure-visual-studio-code/run-debugger.png"::: |
| Click *Run and Debug*, or hit F5 to run the debugger. Then Hover over the variable `name` on line 7 to see its value. Exit the debugger by clicking **Continue** on the debugger bar or hit F5. | :::image type="content" source="./media/configure-visual-studio-code/debug-variable-240px.png" alt-text="A screenshot showing running the debugger in VS code." lightbox="./media/configure-visual-studio-code/debug-variable.png"::: |

## Next steps

> [!div class="nextstepaction"]
> [Key Azure Services for Go Developers](key-azure-services-for-go.md)
> [!div class="nextstepaction"]
> [Authenticate with the Azure SDK for Go](azure-sdk-authentication.md)
