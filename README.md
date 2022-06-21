# Mac Private Server Connect

This repo contains a simple helper script to connect to HoN private servers. Basically it's just an AppleScript to pass the appropriate command
line arguments on mac.

## FAQ

I'm getting one of these errors: `"Apple couldn't verify this app for malware"` or `"This application is damaged and cannot be opened"`.

This is because the HoN team never got past the beta testing stage for their mac binary. It is not code-signed, so Apple cannot verify it.

If you want to get around this error, you can run the following command:

```
xattr -d com.apple.quarantine /Applications/Heroes\ of\ Newerth\ x64.app/
```

Context:

> This application is code signed, but it is *NOT* notarised by apple, and will not be notarised during public beta, so you will most likely experience issues opening it for the first time.
>  It will be notarised on official release, and no extra steps will be needed.
>  If you see a message saying "Couldn't verify itself for malware" Open HoN64 by right clicking and pressing open, instead of just double clicking it, and it should give you an option to Open.
>  It is almost guaranteed you will have issues opening it on Mojave and above, and will usually be a random error such as "Apple couldn't verify this app for malware" or "This application is damaged and cannot be opened" and some others.

*Source: https://forums.heroesofnewerth.com/index.php?/topic/3481-download-hon64-macos-client-public-beta/*
