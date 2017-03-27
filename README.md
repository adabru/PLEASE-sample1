# PLEASE-sample1

JSON for curl:

```
{
  versions: {
    zero: {
      build: {
        base: "alpine",
        full: "apk add --no-cache git \ngit clone git://github.com/adabru/PLEASE-sample1\n chmod +x PLEASE-sample1/start.sh"
      },
      deploy: {
        space: {
          base: "build",
          command: "cd PLEASE-sample1 \n./start.sh",
          widgets: ["$ip4_http/80/widget.xml"]
        }
    }
  }
}
```
