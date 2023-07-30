# aboxes

Run one or more commands on multiple remote hosts via SSH.
This is most commonly used for retrieving ad-hoc information without too much fuzz.

## Usage

```bash
$ aboxes run -t theta,testalex.h -c hostname
INFO[0000] theta: theta
INFO[0000] testalex.h: j6yt29-testalex-magweb-do.nodes.hypernode.io

# Format output with Go template syntax
$ aboxes run -t theta,testalex.h -c hostname --format "{{.Target}} -> {{.Stdout}}"
INFO[0000] theta -> theta
INFO[0000] testalex.h -> j6yt29-testalex-magweb-do.nodes.hypernode.io
```
