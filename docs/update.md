# Update

* Run the following commands to update brond, all dependencies, and install it:

```bash
cd $GOPATH/src/github.com/bronsuite/brond
git pull && GO111MODULE=on go install -v . ./cmd/...
```
