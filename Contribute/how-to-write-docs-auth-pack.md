---
title: Pack zur Dokumenterstellung für VS Code
description: VS Code-Erweiterungspaket zur vereinfachten Markdown-Dokumenterstellung für docs.microsoft.com
author: meganbradley
ms.author: mbradley
manager: jemash
ms.date: 04/06/2018
ms.article: contributor-guide
ms.prod: n.a
ms.service: n.a
ms.technology: n.a
ms.openlocfilehash: 5c857deb07e28e1f6744c895a291bf78a6acf1df
ms.sourcegitcommit: dd1b4e915f4996ac029d2a0704ced785438d3484
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2018
---
# <a name="docs-authoring-pack-for-vs-code"></a><span data-ttu-id="aec38-103">Pack zur Dokumenterstellung für VS Code</span><span class="sxs-lookup"><span data-stu-id="aec38-103">Docs Authoring Pack for VS Code</span></span>

<span data-ttu-id="aec38-104">Das Pack zur Dokumenterstellung ist eine Sammlung von VS Code-Erweiterungen zum vereinfachten Erstellen von Dokumenten für docs.microsoft.com. Das Pack kann im [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=docsmsft.docs-authoring-pack) heruntergeladen werden und enthält die folgenden Erweiterungen:</span><span class="sxs-lookup"><span data-stu-id="aec38-104">The Docs Authoring Pack is a collection of VS Code extensions to aid with Markdown authoring for docs.microsoft.com. The pack is [available in the VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=docsmsft.docs-authoring-pack) and contains the following extensions:</span></span>

- <span data-ttu-id="aec38-105">**DocFX:** Stellt eine Markdownvorschau speziell für docs.microsoft.com zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="aec38-105">**DocFx:** Provides a docs.microsoft.com-specific Markdown preview.</span></span> <span data-ttu-id="aec38-106">Weitere Informationen finden Sie unter [DocFX](https://marketplace.visualstudio.com/items?itemName=ms-docfx.DocFX).</span><span class="sxs-lookup"><span data-stu-id="aec38-106">For more information, see [DocFx](https://marketplace.visualstudio.com/items?itemName=ms-docfx.DocFX).</span></span>
- <span data-ttu-id="aec38-107">**markdownlint:** Beliebter Markdownlinter von David Anson, der die Nutzung bewährter Methoden durch Markdown sicherstellt.</span><span class="sxs-lookup"><span data-stu-id="aec38-107">**markdownlint:** A popular Markdown linter by David Anson to help ensure your Markdown follows best practices.</span></span> <span data-ttu-id="aec38-108">Weitere Informationen finden Sie unter [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint).</span><span class="sxs-lookup"><span data-stu-id="aec38-108">For more information, see [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint).</span></span>
- <span data-ttu-id="aec38-109">**Docs Markdown:** Stellt Unterstützung bei der Markdown-Dokumenterstellung von docs.microsoft.com-Inhalten im Open Publishing System (OPS) bereit, einschließlich Basic-Support für Markdown sowie Unterstützung für benutzerdefinierte Markdownsyntax in OPS.</span><span class="sxs-lookup"><span data-stu-id="aec38-109">**Docs Markdown:** Provides Markdown authoring assistance for docs.microsoft.com content in the Open Publishing System (OPS), including basic Markdown support and support for custom Markdown syntax in OPS.</span></span> <span data-ttu-id="aec38-110">Die weiteren Abschnitte dieses Themas behandeln die Erweiterung „Docs Markdown“.</span><span class="sxs-lookup"><span data-stu-id="aec38-110">The rest of this topic describes the Docs Markdown extension.</span></span>

## <a name="prerequisites-and-assumptions"></a><span data-ttu-id="aec38-111">Voraussetzungen und Annahmen</span><span class="sxs-lookup"><span data-stu-id="aec38-111">Prerequisites and assumptions</span></span>

<span data-ttu-id="aec38-112">Damit Sie relative Links, Images und andere eingebettete Inhalte mit der Erweiterung „Docs Markdown“ korrekt einfügen können, muss der VS Code-Arbeitsbereich dem Stamm Ihres geklonten OPS-Repositorys zugeordnet sein.</span><span class="sxs-lookup"><span data-stu-id="aec38-112">To accurately insert relative links, images, and other embedded content with the Docs Markdown extension, you must have your VS Code workspace scoped to the root of your cloned OPS repo.</span></span>

<span data-ttu-id="aec38-113">Ein Teil der von der Erweiterung unterstützten Syntax, wie z.B. Warnungen und Codeausschnitte, stellt für OPS ein benutzerdefiniertes Markdown dar. Diese Syntax wird daher nur korrekt gerendert, wenn sie über OPS veröffentlicht wird.</span><span class="sxs-lookup"><span data-stu-id="aec38-113">Some syntax supported by the extension, such as alerts and snippets, are custom Markdown for OPS, and will not render correctly unless published via OPS.</span></span>

## <a name="how-to-use-the-docs-markdown-extension"></a><span data-ttu-id="aec38-114">Verwenden der Erweiterung „Docs Markdown“</span><span class="sxs-lookup"><span data-stu-id="aec38-114">How to use the Docs Markdown extension</span></span>

<span data-ttu-id="aec38-115">Drücken Sie `ALT+M`, um auf das Docs Markdown-Menü zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="aec38-115">To access the Docs Markdown menu, type `ALT+M`.</span></span> <span data-ttu-id="aec38-116">Klicken Sie auf die gewünschte Funktion, oder verwenden Sie dazu die NACH-OBEN-/NACH-UNTEN-TASTEN. Sie können zum Filtern auch mit der Eingabe des Namens beginnen und `ENTER` drücken, sobald die gewünschte Funktion im Menü hervorgehoben wird.</span><span class="sxs-lookup"><span data-stu-id="aec38-116">You can click or use up/down arrows to select the function you want, or type to start filtering, then hit `ENTER` when the function you want is highlighted in the menu.</span></span> <span data-ttu-id="aec38-117">Folgende Funktionen sind verfügbar:</span><span class="sxs-lookup"><span data-stu-id="aec38-117">The following are available:</span></span>

|<span data-ttu-id="aec38-118">Funktion</span><span class="sxs-lookup"><span data-stu-id="aec38-118">Function</span></span>     |<span data-ttu-id="aec38-119">Befehl</span><span class="sxs-lookup"><span data-stu-id="aec38-119">Command</span></span>             |<span data-ttu-id="aec38-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aec38-120">Description</span></span>           |
|-------------|--------------------|----------------------|
|<span data-ttu-id="aec38-121">Fett</span><span class="sxs-lookup"><span data-stu-id="aec38-121">Bold</span></span>         |`formatBold`        |<span data-ttu-id="aec38-122">Text wird **fett** formatiert.</span><span class="sxs-lookup"><span data-stu-id="aec38-122">Formats text **bold**.</span></span>|
|<span data-ttu-id="aec38-123">Kursiv</span><span class="sxs-lookup"><span data-stu-id="aec38-123">Italic</span></span>       |`formatItalic`      |<span data-ttu-id="aec38-124">Text wird *kursiv* formatiert.</span><span class="sxs-lookup"><span data-stu-id="aec38-124">Formats text *italic*.</span></span>|
|<span data-ttu-id="aec38-125">Code</span><span class="sxs-lookup"><span data-stu-id="aec38-125">Code</span></span>         |`formatCode`        |<span data-ttu-id="aec38-126">Text wird als `inline code` formatiert, wenn höchstens eine Zeile ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="aec38-126">If one line or less is selected, formats text as `inline code`.</span></span><br><br><span data-ttu-id="aec38-127">Bei mehreren ausgewählten Zeilen werden diese als umgrenzter Codeblock formatiert. Sie können in diesem Fall optional auch eine von OPS unterstützte Programmiersprache festlegen.</span><span class="sxs-lookup"><span data-stu-id="aec38-127">If multiple lines are selected, formats them as a fenced code block, and allows you to optionally select a programming language supported by OPS.</span></span>|
|<span data-ttu-id="aec38-128">Warnung</span><span class="sxs-lookup"><span data-stu-id="aec38-128">Alert</span></span>        |`insertAlert`       |<span data-ttu-id="aec38-129">Es wird „Hinweis“, „Wichtig“, „Warnung“ oder „Tipp“ eingefügt.</span><span class="sxs-lookup"><span data-stu-id="aec38-129">Inserts a Note, Important, Warning, or Tip.</span></span><br><br><span data-ttu-id="aec38-130">Klicken Sie im Menü auf „Warnung“, und wählen Sie anschließend den Warnungstyp aus.</span><span class="sxs-lookup"><span data-stu-id="aec38-130">Select Alert from the menu, then select the alert type.</span></span> <span data-ttu-id="aec38-131">Bereits ausgewählter Text wird in die Syntax der ausgewählten Warnung eingeschlossen.</span><span class="sxs-lookup"><span data-stu-id="aec38-131">If you have previously selected text, it will be surrounded with the selected alert syntax.</span></span> <span data-ttu-id="aec38-132">Wenn Sie noch keinen Text ausgewählt haben, wird eine neue Warnung mit Platzhaltertext hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aec38-132">If no text is selected, a new alert will be added with placeholder text.</span></span>|
|<span data-ttu-id="aec38-133">Nummerierte Liste</span><span class="sxs-lookup"><span data-stu-id="aec38-133">Numbered list</span></span>|`insertNumberedList` |<span data-ttu-id="aec38-134">Eine nummerierte Liste wird eingefügt.</span><span class="sxs-lookup"><span data-stu-id="aec38-134">Inserts a new numbered list.</span></span><br><br> <span data-ttu-id="aec38-135">Bei mehreren ausgewählten Zeilen wird jede Zeile zu einem Element der Liste.</span><span class="sxs-lookup"><span data-stu-id="aec38-135">If multiple lines are selected, each will be a list item.</span></span> <span data-ttu-id="aec38-136">Beachten Sie, dass bei nummerierten Listen alle Elemente im Markdown mit einer 1 angezeigt werden. Auf docs.microsoft.com werden sie hingegen als fortlaufende Zahlen oder bei geschachtelten Listen als Buchstaben gerendert.</span><span class="sxs-lookup"><span data-stu-id="aec38-136">Note that numbered lists show in the Markdown as all 1s, but will render on docs.microsoft.com as sequential numbers or, for nested lists, letters.</span></span> <span data-ttu-id="aec38-137">Verwenden Sie zum Erstellen einer geschachtelten nummerierten Liste den Tabstopp innerhalb der übergeordneten Liste.</span><span class="sxs-lookup"><span data-stu-id="aec38-137">To create a nested numbered list, tab from within the parent list.</span></span>|
|<span data-ttu-id="aec38-138">Liste mit Aufzählungszeichen</span><span class="sxs-lookup"><span data-stu-id="aec38-138">Bulleted list</span></span>|`insertBulletedList` |<span data-ttu-id="aec38-139">Eine Liste mit Aufzählungszeichen wird eingefügt.</span><span class="sxs-lookup"><span data-stu-id="aec38-139">Inserts a new bulleted list.</span></span>|
|<span data-ttu-id="aec38-140">Tabelle</span><span class="sxs-lookup"><span data-stu-id="aec38-140">Table</span></span>        |`insertTable`        |<span data-ttu-id="aec38-141">Eine Markdown-Tabellenstruktur wird eingefügt.</span><span class="sxs-lookup"><span data-stu-id="aec38-141">Inserts a Markdown table structure.</span></span><br><br><span data-ttu-id="aec38-142">Geben Sie nach dem Auswählen des Befehls „Tabelle“ die Anzahl der Spalten und Zeilen im Format „Spalten:Zeilen“ an, z.B. „3:4“.</span><span class="sxs-lookup"><span data-stu-id="aec38-142">After you select the table command, specify the number of columns and rows in the format columns:rows, such as 3:4.</span></span> <span data-ttu-id="aec38-143">Beachten Sie, dass die maximale Spaltenanzahl, die mithilfe der Erweiterung angegeben werden kann, 5 beträgt. Dies ist auch die empfohlene Höchstzahl für Spalten, um eine optimale Lesbarkeit zu gewährleisten.</span><span class="sxs-lookup"><span data-stu-id="aec38-143">Note that the maximum number of columns you can specify via this extension is 5, which is the recommended maximum for readability.</span></span>|
|<span data-ttu-id="aec38-144">Link</span><span class="sxs-lookup"><span data-stu-id="aec38-144">Link</span></span>         |`selectLinkType`      |<span data-ttu-id="aec38-145">Ein Link wird eingefügt.</span><span class="sxs-lookup"><span data-stu-id="aec38-145">Inserts a link.</span></span> <span data-ttu-id="aec38-146">Wenn Sie diesen Befehl auswählen, wird das folgende Untermenü angezeigt:</span><span class="sxs-lookup"><span data-stu-id="aec38-146">When you select this command, the following sub-menu appears.</span></span><br><br><span data-ttu-id="aec38-147">`External`: Link zu einer Webseite über den URI.</span><span class="sxs-lookup"><span data-stu-id="aec38-147">`External`: Link to a web page by URI.</span></span> <span data-ttu-id="aec38-148">Muss „http“ oder „https“ beinhalten.</span><span class="sxs-lookup"><span data-stu-id="aec38-148">Must include "http" or "https".</span></span><br><span data-ttu-id="aec38-149">`Internal`: Relativer Link zu einer anderen Datei im selben Repository.</span><span class="sxs-lookup"><span data-stu-id="aec38-149">`Internal`: Insert a relative link to another file in the same repo.</span></span> <span data-ttu-id="aec38-150">Nachdem Sie diese Option ausgewählt haben, geben Sie im Befehlsfenster Text ein, um die Dateien nach Namen zu filtern. Klicken Sie anschließend auf die gewünschte Datei.</span><span class="sxs-lookup"><span data-stu-id="aec38-150">After selecting this option, type in the command window to filter files by name, then select the file you want.</span></span> <br><span data-ttu-id="aec38-151">`Bookmark in this file`: Treffen Sie in der aktuellen Datei in einer Liste mit Überschriften eine Auswahl, um ein korrekt formatiertes Lesezeichen einzufügen.</span><span class="sxs-lookup"><span data-stu-id="aec38-151">`Bookmark in this file`: Choose from a list of headings in the current file to insert a properly formatted bookmark.</span></span><br><span data-ttu-id="aec38-152">`Bookmark in another file`: Filtern Sie zunächst nach Dateinamen, und wählen Sie die Datei aus, auf die der Link verweisen soll. Wählen Sie dann die entsprechende Überschrift in der ausgewählten Datei aus.</span><span class="sxs-lookup"><span data-stu-id="aec38-152">`Bookmark in another file`: First, filter by file name and select the file to link to, then choose the appropriate heading within the selected file.</span></span>|
|<span data-ttu-id="aec38-153">Image</span><span class="sxs-lookup"><span data-stu-id="aec38-153">Image</span></span>        |`insertImage`     |<span data-ttu-id="aec38-154">Geben Sie Alternativtext ein (für die Barrierefreiheit erforderlich), und wählen Sie ihn aus. Rufen Sie dann diesen Befehl auf, um die Liste der unterstützten Bilddateien im Repository zu filtern, und wählen Sie die gewünschte Datei aus.</span><span class="sxs-lookup"><span data-stu-id="aec38-154">Type alternate text (required for accessibility) and select it, then call this command to filter the list of supported image files in the repo and select the one you want.</span></span> <span data-ttu-id="aec38-155">Wenn Sie beim Aufrufen dieses Befehls keinen Alternativtext ausgewählt haben, werden Sie zu einer Eingabe aufgefordert, bevor Sie die Bilddatei auswählen können.</span><span class="sxs-lookup"><span data-stu-id="aec38-155">If you haven't selected alt text when you call this command, you will be prompted for it before you can select an image file.</span></span>|
|<span data-ttu-id="aec38-156">Einschließen</span><span class="sxs-lookup"><span data-stu-id="aec38-156">Include</span></span>      |`insertInclude`   |<span data-ttu-id="aec38-157">Eine Datei wird gesucht, die in die aktuelle Datei eingebettet werden soll.</span><span class="sxs-lookup"><span data-stu-id="aec38-157">Find a file to embed in the current file.</span></span>|
|<span data-ttu-id="aec38-158">Codeausschnitt</span><span class="sxs-lookup"><span data-stu-id="aec38-158">Snippet</span></span>      |`insertSnippet`   |<span data-ttu-id="aec38-159">Im Repository wird ein Codeausschnitt gesucht, der in die aktuelle Datei eingebettet werden soll.</span><span class="sxs-lookup"><span data-stu-id="aec38-159">Find a code snippet in the repo to embed in the current file.</span></span>|
|<span data-ttu-id="aec38-160">Bewegte Bilder</span><span class="sxs-lookup"><span data-stu-id="aec38-160">Video</span></span>        |`insertVideo`     |<span data-ttu-id="aec38-161">Ein eingebettetes Video wird hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aec38-161">Add an embedded video.</span></span>|
|<span data-ttu-id="aec38-162">Vorschau</span><span class="sxs-lookup"><span data-stu-id="aec38-162">Preview</span></span>      |`previewTopic`    |<span data-ttu-id="aec38-163">Mithilfe der Erweiterung „DocFX“ wird das aktive Thema in einem Vorschaufenster parallel angezeigt.</span><span class="sxs-lookup"><span data-stu-id="aec38-163">Preview the active topic in a side-by-side window using the DocFX extension.</span></span>  <span data-ttu-id="aec38-164">Wenn die Erweiterung „DocFX“ nicht installiert ist, oder wenn sie zwar installiert jedoch deaktiviert ist, wird das Thema nicht gerendert.</span><span class="sxs-lookup"><span data-stu-id="aec38-164">If the DocFX extension is not installed or is installed but disabled, the topic will not render.</span></span>


## <a name="how-to-assign-keyboard-shortcuts"></a><span data-ttu-id="aec38-165">Zuweisen von Tastenkombinationen</span><span class="sxs-lookup"><span data-stu-id="aec38-165">How to assign keyboard shortcuts</span></span>

1. <span data-ttu-id="aec38-166">Drücken Sie zum Öffnen der Liste mit den Tastenkombinationen zuerst `CTRL+K` und anschließend `CTRL+S`.</span><span class="sxs-lookup"><span data-stu-id="aec38-166">Type `CTRL+K` then `CTRL+S` to open the Keyboard Shortcuts list.</span></span>
1. <span data-ttu-id="aec38-167">Suchen Sie den Befehl, z.B. `formatBold`, für den Sie eine benutzerdefinierte Tastenzuordnung erstellen möchten.</span><span class="sxs-lookup"><span data-stu-id="aec38-167">Search for the command, such as `formatBold`, for which you want to create a custom keybinding.</span></span>
1. <span data-ttu-id="aec38-168">Klicken Sie auf das Pluszeichen, das neben dem Befehlsnamen angezeigt wird, wenn Sie mit der Maus auf die Zeile zeigen.</span><span class="sxs-lookup"><span data-stu-id="aec38-168">Click the plus that appears near the command name when you mouse over the line.</span></span>
1. <span data-ttu-id="aec38-169">Geben Sie in das neu angezeigte Eingabefeld die Tastenkombination ein, die mit diesem bestimmten Befehl verknüpft werden soll.</span><span class="sxs-lookup"><span data-stu-id="aec38-169">After a new input box is visible, type the keyboard shortcut you want to bind to that particular command.</span></span> <span data-ttu-id="aec38-170">Geben Sie z.B. `ctrl+b` ein, um die gängige Tastenkombination für Fettdruck zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="aec38-170">For example, to use the common shortcut for bold, type `ctrl+b`.</span></span>
1. <span data-ttu-id="aec38-171">Es wird empfohlen, in die Tastenzuordnung eine `when`-Klausel einzufügen, damit die Zuordnung nur in Markdowndateien verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="aec38-171">It's a good idea to insert a `when` clause into your keybinding, so it won't be available in files other than Markdown.</span></span> <span data-ttu-id="aec38-172">Öffnen Sie hierzu *keybindings.json*, und fügen Sie die folgende Zeile unterhalb des Befehlsnamens ein (achten Sie dabei auf das Komma zwischen den Zeilen):</span><span class="sxs-lookup"><span data-stu-id="aec38-172">To do this, open *keybindings.json* and insert the following line below the command name (be sure to add a comma between lines):</span></span>
   
    `"when": "editorTextFocus && editorLangId == 'markdown'"`

    <span data-ttu-id="aec38-173">Die fertige benutzerdefinierte Tastenzuordnung sollte in „keybindings.json“ wie folgt aussehen:</span><span class="sxs-lookup"><span data-stu-id="aec38-173">Your completed custom keybinding should look like this in keybindings.json:</span></span>

    ```json
    // Place your key bindings in this file to overwrite the defaults
    [
        {
            "key": "ctrl+b",
            "command": "formatBold",
            "when": "editorTextFocus && editorLangId == 'markdown'"
        }
    ]
    ```

1. <span data-ttu-id="aec38-174">Speichern Sie die Datei „keybindings.json“.</span><span class="sxs-lookup"><span data-stu-id="aec38-174">Save keybindings.json.</span></span>

<span data-ttu-id="aec38-175">Weitere Informationen finden Sie unter [Keybindings (Tastenzuordnungen)](https://code.visualstudio.com/docs/getstarted/keybindings) in der VS Code-Dokumentation.</span><span class="sxs-lookup"><span data-stu-id="aec38-175">See [Keybindings](https://code.visualstudio.com/docs/getstarted/keybindings) in the VS Code docs for more information.</span></span>

## <a name="how-to-show-the-legacy-gauntlet-toolbar"></a><span data-ttu-id="aec38-176">Anzeigen der Symbolleiste „Gauntlet“ der Vorgängerversion</span><span class="sxs-lookup"><span data-stu-id="aec38-176">How to show the legacy "Gauntlet" toolbar</span></span>

<span data-ttu-id="aec38-177">Die Symbolleiste zur Dokumenterstellung aus dem Erweiterungscode „Gauntlet“ der Vorgängerversion wird nicht mehr unten im VS Code-Fenster angezeigt, wenn die Erweiterung „Docs Markdown“ installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="aec38-177">Former users of the extension code-named "Gauntlet" will notice that the authoring toolbar no longer appears at the bottom of the VS Code window when the Docs Markdown Extension is installed.</span></span> <span data-ttu-id="aec38-178">Dies liegt daran, dass die Symbolleiste in der VS Code-Statusleiste viel Platz in Anspruch nahm und nicht den bewährten Methoden für Benutzerfreundlichkeit entsprach, weshalb sie in der neuen Erweiterung verworfen wurde.</span><span class="sxs-lookup"><span data-stu-id="aec38-178">This is because the toolbar took up a lot of space on the VS Code status bar and did not follow best practices for extension UX, so it is deprecated in the new extension.</span></span> <span data-ttu-id="aec38-179">Sie können die Symbolleiste jedoch optional anzeigen, indem Sie die VS Code-Datei „settings.json“ wie folgt aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="aec38-179">However, you can optionally show the toolbar by updating your VS Code settings.json file as follows:</span></span>

1. <span data-ttu-id="aec38-180">Gehen Sie in VS Code zu „Datei“ > „Einstellungen“ > „Einstellungen“ (`CTRL+Comma`).</span><span class="sxs-lookup"><span data-stu-id="aec38-180">In VS Code, go to File -> Preferences -> Settings (`CTRL+Comma`).</span></span>
1. <span data-ttu-id="aec38-181">Wählen Sie „Benutzereinstellungen“ aus, um die Einstellungen für sämtliche VS Code-Arbeitsbereiche zu ändern, oder „Arbeitsbereichseinstellungen“, um nur die Einstellungen für den aktuellen Arbeitsbereich zu ändern.</span><span class="sxs-lookup"><span data-stu-id="aec38-181">Select User Settings to change the settings for all VS Code workspaces, or  Workspace Settings to change them for just the current workspace.</span></span>
1. <span data-ttu-id="aec38-182">Suchen Sie im Bereich „Standardeinstellungen“ nach der Konfiguration für die Erweiterung „Docs Authoring“, und klicken Sie auf das Bleistiftsymbol neben der gewünschten Einstellung.</span><span class="sxs-lookup"><span data-stu-id="aec38-182">In the Default Settings pane, find Docs Authoring Extension Configuration, and select the pencil icon next to the desired setting.</span></span> <span data-ttu-id="aec38-183">Als Nächstes werden Sie aufgefordert, `true` oder `false` auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="aec38-183">Next, you will be prompted to select either `true` or `false`.</span></span> <span data-ttu-id="aec38-184">Anschließend wird der Wert durch VS Code automatisch der Datei „settings.json“ hinzugefügt. Sie werden nun aufgefordert, das Fenster erneut zu laden, damit die Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="aec38-184">Once you've made your selection, VS Code will automatically add the value to the settings.json file and you will be prompted to reload the window for the changes to take effect.</span></span>

## <a name="known-issues"></a><span data-ttu-id="aec38-185">Bekannte Probleme</span><span class="sxs-lookup"><span data-stu-id="aec38-185">Known issues</span></span>

- <span data-ttu-id="aec38-186">[DocFX Preview]: MacOS und Linux: Die Vorschau wird von DocFX Preview nicht korrekt gestartet (die Standardvorschau für diese Plattformen lautet „VS Code Markdown-Vorschau“).</span><span class="sxs-lookup"><span data-stu-id="aec38-186">[DocFX Preview] MacOS and Linux: DocFX Preview does not launch preview correctly (preview defaults to VS Code Markdown preview for these platforms).</span></span>
- <span data-ttu-id="aec38-187">[DocFX Preview]: Alle Plattformen: Ein Teil der Syntax, z.B. XRef-Links (Querverweise) zu APIs, wird in der Vorschau nicht korrekt gerendert, wodurch in einigen Fällen Lücken im Inhalt entstehen.</span><span class="sxs-lookup"><span data-stu-id="aec38-187">[DocFx Preview] All platforms: Some syntax, such as xref (cross-reference) links to APIs, do not render correctly in preview, in some cases leaving content gaps.</span></span>
- <span data-ttu-id="aec38-188">[External bookmarks]: Linux: Die Dateiliste wird angezeigt, jedoch keine Überschriften, die ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="aec38-188">[External bookmarks] Linux: File list is displayed but no headings are shown to select.</span></span>
- <span data-ttu-id="aec38-189">[Includes]: Linux: Die Dateiliste wird angezeigt, doch nach der Auswahl wird kein Link hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="aec38-189">[Includes] Linux: File list is displayed but no link is added after selection is made.</span></span>