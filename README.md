# kiwiの準備
下記を実行し必要な環境を準備する。
```
sudo zypper install python3-kiwi
sudo zypper install python3-xmltodict
git clone https://github.com/OSInside/kiwi.git
git clone https://github.com/aruelu/mykiwi.git
```

# kiwi設定ファイル

パスワードは変更してビルドして下さい。

- test-gui-01：./kiwi/build-tests/x86/tumbleweed/test-image-diskを元にkiwiファイルを修正
- test-gui-02：gnomeデスクトップ

## ビルド方法
```
sudo kiwi-ng system build --description mykiwi/test-gui-01 --target-dir iso-gui-01 --set-repo obs://openSUSE:Tumbleweed/standard
```
ディレクトリ名は、ビルドしたいkiwiファイルの入っている名称に変更して下さい。
