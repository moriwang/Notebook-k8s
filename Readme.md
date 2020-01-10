## How to release new version

推送 tag 后，docker hub 将自动建构新版本。
https://hub.docker.com/r/zesheng/base-notebook-k8s

### how to push tags
```
# git tag -a 标签名 -m 标签说明
git tag -a v0.0.1 -m 'tagging version 0.0.1'

# 推送标签
git push origin --tags
```

### delete local and remote tags
```
# 删除本地标签
git tag -d v0.0.1

# 删除仓库标签
git push origin :refs/tags/v0.0.1
```