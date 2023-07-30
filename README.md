# kicad-template

このテンプレート使用の際はリポジトリクローン後に以下のコマンドを実行.

```
zsh init
```

コマンド実行後、以下の処理が走り、kicad 開発環境を自動生成する

1. 各種作業ファイル生成

   `Untitled`になっている`kicad_pcb`, `kicad_pro`, `kicad_sch`の 3 ファイルをプロジェクト名に変更

2. KiCad のフットプリント・シンボルライブラリのクローン

   以下 3 つのリポジトリをサブモジュールとしてクローンする

- https://github.com/njl7502l/njl7502l-kicad-library
- https://github.com/Digi-Key/digikey-kicad-library
- https://github.com/espressif/kicad-libraries/

3. シンボルライブラリテーブルの自動生成

   digikey のシンボルライブラリは更新によって数が増減するかもしれないので、clone 毎に関連付けを自動生成する

4. github への push
