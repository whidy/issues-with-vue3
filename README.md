# Vue project with Volar formatting error

```
error info:
[Error - 3:00:18 PM] Request textDocument/formatting failed.
  Message: Request textDocument/formatting failed with message: Overlapping edit
  Code: -32603
```

git clone, open file `src/App.vue` .

with macOS, as default code, `option + shift + f` works well.

now, try to go line `34~38` (script section), any line end input a space or enter. Then press `option + shift + f` will trigger error. But in template section, edit something, try to `option + shift + f` again, every thing go well again.

watch the video: https://youtu.be/BB92-GNgmmQ
