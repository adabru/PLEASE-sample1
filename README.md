# PLEASE-sample1

JSON for curl:

```
{
  versions: {
    zero: {
      build: {
        base: "alpine",
        full: "apk add --no-cache git && git clone git://github.com/adabru/PLEASE-sample1"
      },
      deploy: {
        space: {
          base: "build",
          command: "./start.sh"
        }
    }
  }
}
```
