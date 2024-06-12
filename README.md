# openapi-test-public2

openapiのテスト。public リポジトリのため注意。

## 設定

rbenvでlocal設定

```shell
rbenv local $(cat .ruby-version)
```

bundlerとjekyllをインストール

```shell
gem install bundler jekyll
```

bundle install

```shell
bundle install
```

## ビルド

_site内にビルド

```shell
bundle exec jekyll build -s docs --config docs/_config_development.yml
```

<http://localhost:4000>に表示。ビルドも同時に行う。

```shell
bundle exec jekyll serve -s docs --config docs/_config_development.yml
```
