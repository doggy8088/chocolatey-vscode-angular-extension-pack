## Angular Extension Pack for Visual Studio Code

This extension pack packages some of the most popular (and some of my favorite) Angular extensions. If you like it, please leave your Rating & Review and share with your friends. If you know any extension that is good for Angular development, just let me know by creating an issue.

### How to build package

```sh
choco pack
```

### How to test install locally

```sh
choco install vscode-angular-extension-pack -d -s .
```

### How to test uninstall locally

```sh
choco uninstall vscode-angular-extension-pack -d -s .
```

### How to update this package

1. Edit `vscode-angular-extension-pack.nuspec`

    * Update `<version>`
    * Update `<releaseNotes>` (reference from [here](https://raw.githubusercontent.com/go-gitea/gitea/master/CHANGELOG.md))

2. Test install

    ```sh
    choco pack
    choco install vscode-angular-extension-pack -d -s . -y
    choco uninstall vscode-angular-extension-pack -d -s .
    ```

3. Publish to Chocolatey Gallery

    ```sh
    choco push vscode-angular-extension-pack.X.Y.Z.nupkg --source https://push.chocolatey.org/ --apikey YourChocolateyApiKey
    ```
