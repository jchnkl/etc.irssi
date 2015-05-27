Keep the config free of passwords

In `$GIT_DIR/info/attributes`:

    config filter=pw

In `$GIT_DIR/config`:

    [filter "pw"]
      clean = "sed -e 's/identify .*\";/identify <PASSWORD>\";/'"
