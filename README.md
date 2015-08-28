# Android CI check Gradle

## 使い方

モジュールの`build.gradle`に下記を追加します。

```groovy
apply from: "https://raw.githubusercontent.com/monstar-lab/gradle-android-ci-check/1.2.0/ci.gradle"
```

## 拡張性

### チェックルールの変更

このリポジトリに格納されている`checkstyle.xml`や`findbugs-filter.xml`をダウンロードし、修正します。

プロジェクト内に格納し、モジュールの`build.gradle`にさらに追記します。

```
checkStyleConfigFile=../config/quality/checkstyle/checkstyle.xml
findBugsExcludeFilter=../config/quality/findbugs/findbugs-filter.xml
```
