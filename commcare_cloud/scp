# SCP File from CommCare host to local

For simple, single-files:

```
cchq --control <env> ssh django_manage 'sudo -u cchq cat /home/cchq/some_file.json' > ./some_file.json
```

Or, if it's particularly large and compressible, gzip can reduce over-the-wire bandwidth:

```
cchq --control <env> ssh django_manage 'sudo -u cchq gzip -c /home/cchq/some_file.json' | gzip -cd > ./some_file.json
```
