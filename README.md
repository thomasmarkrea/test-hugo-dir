>
> This issue has been resolved  
> https://github.com/gohugoio/hugo/issues/7589
>

---


# Test Hugo .Dir

Used from a standard archetype `.File.Dir` returns a path relative to `content/`.

Used from a directory based archetype `.File.Dir` returns the absolute path.

A relative path is the expected behaviour.

## Test

```bash
git clone https://github.com/thomasmarkrea/test-hugo-dir.git
cd test-hugo-dir/

hugo new -k test blog/test.md
hugo new -k test-bundle blog/test
```

## Hugo Environment

```bash
hugo env
Hugo Static Site Generator v0.72.0-8A7EF3CF/extended linux/amd64 BuildDate: 2020-05-31T12:14:23Z
GOOS="linux"
GOARCH="amd64"
GOVERSION="go1.14.3"
```