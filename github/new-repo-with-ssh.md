

After creating new repo you have to set remote url. If you want to authenticate with ssh do the following: 

```
git remote set-url origin git@github.com:<Username>/<Project>.git
```
and
```
git push -u origin main
```

After generating ssh, add it to keychain: 
```
ssh-add --apple-use-keychain ~/.ssh/github/github-private
```