## steep のテスト
gem に添付されている sig ディレクトリ以下の rbs ファイルをもとに steep で型チェックする

```
$ bundle install
$ bundle exec steep check
lib/main.rb:4:30: ArgumentTypeMismatch: receiver=singleton(::SlackAlphabetter), expected=::String, actual=::Integer (123)
```