# leech

`leech` is a simple Bash script that reads URLs and opens them in various programs. You can let XDG handle a local download of of the URL's content using MIME types or assign programs to specific URL patterns by using a `leechtab`.

The intended use for leech is to be used as a minimalist, suckless-inspired way of using the web by decoupling the tight integration of technologies as found in modern web browsers and leave all your visited websites to programs that do one thing and do it well.

## Dependencies

- `xdg-open`
- `curl`
- `sponge` from `moreutils`

## leechtab

The leechtab is rather simple: All you have to do is create a file in you XDG config or data directory (or alternatively create `~/.leechtab`) for example the line

```
youtube.com/watch	vlc
```

will cause leech to catch any YouTube video link and play it through VLC.
