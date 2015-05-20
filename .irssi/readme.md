Keep the config free of passwords

In `.gitattributes`:

    config filter=pw

In `.git/config`:

    [filter "pw"]
      clean = "sed -e 's/identify .*\";/identify <PASSWORD>\";/'"
