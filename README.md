
If you are working these days in iOS development you may be using multiple versions of Xcode. (6.4, 7.0-GM, 7.1-beta,....). And since they all have the same icon and there wasn't big changes on the UI it is quite easy to mix them up.

With these tips you could palliate the problem:


# Red icon for Xcode-beta

Copy the file XCodeBeta.icns that you can find in this repo to /Applications/Xcode-beta.app/Contents/Resources/XcodeBeta.icns

```
$ git clone https://github.com/dcordero/BetafyXcode.git
$ cp BetafyXcode/XcodeBeta.icns /Applications/Xcode-beta.app/Contents/Resources/XcodeBeta.icns
```

![](Preview.png)

# Aliases

Since using the command `open` has a random behavior when there are multiple versions of Xcode installed in the system, you could use these two aliases instead. Just adding them to your `~/.bash_profile` they will be available in every terminal session.

```
alias xcode = 'open -a xcode'
alias xcode-beta = 'open -a xcode-beta'
```

