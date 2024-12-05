## License

All the original content (posts and pages) is Copyright Julian Yap.

All other directories and files are MIT Licensed.

## Local development

Serve:
```
hugo server
```

Browse to: http://localhost:1313

New post:
```
hugo new posts/$(date "+%F-%s").md
```

Initialize, fetch and checkout nested submodules (themes):
```
git submodule update --init --recursive
```

Update submodules (themes):
```
git submodule update --remote --recursive
```

Update theme commit:
```
cd themes/${THEME}/
git fetch
git checkout ${SUBMODULE COMMIT}
cd ../
git commit -am "Update theme"
```
