# Downloading and Opening

To use the Scratch projects in this repository, you'll need to download them and open them in a compatible Scratch editor. No software or setup is strictly necessary, other than your web browser, which I'm assuming you already have.

## 1. Download

There are multiple different ways to go about downloading, depending on your needs. You can [download individual files](https://github.com/DNin01/Scratch-projects/blob/main/INSTALLING.md#download-individual-projects-through-the-website) or [an archive of the entire repository](https://github.com/DNin01/Scratch-projects/blob/main/INSTALLING.md#download-the-repository-contents-as-a-zip-archive), or you can [clone it with Git](https://github.com/DNin01/Scratch-projects/blob/main/INSTALLING.md#clone-the-repository-with-git).

### Download individual projects through the website

This is the easiest way to get going if you just want a few projects from time to time.

To do this, simply navigate to the `.sb3` file you want in the Code tab and click the download button. For example, to download Drag Across Windows, navigate to `turbowarp` → `proofs-of-concepts` → `drag-across-windows` → `Drag Across Windows.sb3` then click the download button.

> [!NOTE]
> You will need to repeat this manually whenever the projects are updated.

### Download the repository contents as a ZIP archive

If you want to download everything at once to have, you can download an archive of the entire repository by navigating to the Code tab, opening the "Code" dropdown, then clicking "Download ZIP".

After downloading the archive, extract the `.sb3` file you want.

> [!NOTE]
> You will need to repeat this manually whenever the projects are updated.

### Clone the repository with Git

Prerequisites:
- You'll need to install [Git](https://git-scm.com/). You can also [use GitHub Desktop](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/adding-and-cloning-repositories/cloning-a-repository-from-github-to-github-desktop) if you'd rather work with a GUI.

If you want something a little faster, you can use Git to [clone the repository](https://docs.github.com/en/get-started/using-git/getting-changes-from-a-remote-repository). You can even [ask Git to pull changes](https://docs.github.com/en/get-started/using-git/getting-changes-from-a-remote-repository#pulling-changes-from-a-remote-repository) and it will do the rest - much more convenient than redownloading, extracting, and overwriting manually just to get updates.

## 2. Run

Now we just need a project player to run the projects.

### Opening Scratch projects with TurboWarp extensions

All of the projects in the `turbowarp` directory need to be opened in [TurboWarp](https://turbowarp.org), as these ones use features exclusive to TurboWarp such as [custom extensions](https://extensions.turbowarp.org/). Once you're on TurboWarp, click "File" then "Load from your computer". From there, select the `.sb3` file you want to open.

### If you get an error...

#### Check that the extension is up to date

If you decide to use [TurboWarp Desktop](https://desktop.turbowarp.org/), be aware that it **comes with a copy** of all extensions from the official [TurboWarp Extension Gallery](https://extensions.turbowarp.org/). This means that they work offline but might be outdated. Try again on the website or try updating TurboWarp Desktop.

#### Don't double-click the file!

It's super easy to just open your file manager and double-click by habit and be done, but it won't work for these. Unless you have set `.sb3` files to open in the correct app, you're probably going to encounter some sort of error or not be able to open the projects.

If you would like it to be as easy as double-clicking the file, set them to open in TurboWarp Desktop first.

#### Make sure you're connected

Content filters or issues with internet connection or the TurboWarp Extension Gallery at [extensions.turbowarp.org](https://extensions.turbowarp.org) can prevent the extensions the projects depend on from loading, and the project will subsequently fail to load.

If you're having issues fetching the extensions, another way to load them is through [TurboWarp Desktop](https://desktop.turbowarp.org/). Being an offline app, it comes bundled with a copy of all of the extensions in the gallery.

> [!WARNING]
> As the desktop app comes with a copy of the extensions in the gallery, they may be outdated and not work in some projects. For the best results, update to the latest version.

</details>
