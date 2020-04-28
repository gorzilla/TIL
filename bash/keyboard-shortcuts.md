---------
bash readlines
---------

Have you ever actually sat and read through the bash docs? Neither have I.
There's a whole bunch of weird stuff in there though. I'm sticking it here for personal reference and because these obscure little functions sometimes turn out to have security implications.

- `ctrl a` start of line
- `ctrl e` end of line
- `ctrl c` cancel signal
- `crtl d` eof signal
- `ctrl k` kill (cut) to end of command
- `ctrl y` yank (paste)
- `ctrl r` search through bash history (that's a whole other thing)
- `alt .` last argument
- `alt+#` repeat next char n times

so `alt+50` would repeat the next char 50 times

if you give it a negative argument (`alt -`) it does things backwards
`alt -1` then `ctrl k` cuts to the start of the line

there's some that work on a per word basis but i can't see it saving enough time to be worth remembering

---

[Oh, here's a better way to show it](https://clementc.github.io/blog/2018/01/25/moving_cli/)

![cli cheatsheet](https://clementc.github.io/figures/moving_cli.png)


As long as I'm just linking other people's stuff here's b0rk
![julia evans' bash tricks](https://i.stack.imgur.com/RjLje.jpg)