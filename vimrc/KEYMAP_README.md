Vim keymapping
==============
.vimrcで設定しているキーマップと機能の対応表です

# 画面周り
|キー|デフォルト|機能|モード|
|:---:|:---:|:---:|:---:|
|\||:vsplit\<Cr\>|画面を横方向に分割|ノーマル|
|-|:split\<Cr\>|画面を縦方向に分割|ノーマル|
|\<C-k\>|\<C-w\>k|上の画面へ移動|ノーマル|
|\<C-j\>|\<C-w\>j|下の画面へ移動|ノーマル|
|\<C-l\>|\<C-w\>l|右の画面へ移動|ノーマル|
|\<C-h\>|\<C-w\>h|左の画面へ移動|ノーマル|
|wk|\<C-w\>K|上の画面と入れ替え|ノーマル|
|wj|\<C-w\>J|下の画面と入れ替え|ノーマル|
|wl|\<C-w\>L|右の画面と入れ替え|ノーマル|
|wh|\<C-w\>H|左の画面と入れ替え|ノーマル|
|=|\<C-w\>=|画面幅と画面高を均等に整え|ノーマル|
|\>|\<C-w\>\>|画面幅を拡大|ノーマル|
|\<|\<C-w\>\<|画面幅を縮小|ノーマル|
|^|\<C-w\>+|画面高を拡大|ノーマル|
|\_|\<C-w\>-|画面高を縮小|ノーマル|
|\<C-t\>|:tabnew\<Cr\>|新規タブを作成|ノーマル|
|\<C-n\>|gt|次のタブへ移動|ノーマル|
|\<C-p\>|gT|前のタブへ移動|ノーマル|

# Filer
|キー|デフォルト|機能|モード|
|:---:|:---:|:---:|:---:|
|fo|:VimFiler -split -winwidth=30 -simple -toggle\<Cr\>|ファイラをサイドバーとして開閉|ノーマル|
|ft|:VimFilerTab\<Cr\>|ファイラを新しいタブで開く|ノーマル|

# 入力補完
|キー|デフォルト|機能|モード|
|:---:|:---:|:---:|:---:|
|\<Tab\>||次の候補を選択|インサート|
|\<S-Tab\>||前の候補を選択|インサート|
|\<Cr\>||選択されている候補を入力|インサート|
|\<C-y\>||補完ウィンドウを閉じる|インサート|
|\<C-e\>||補完をキャンセル|インサート|
|\<C-k\>||スニペット補完|インサート＋ヴィジュアル|

# タグジャンプ
|キー|デフォルト|機能|モード|
|:---:|:---:|:---:|:---:|
|tg|:Ctags|タグジャンプに必要なtagsファイルを生成|ノーマル|
|\<C-d\>|\<C-]\>|呼び出し元へジャンプ|ノーマル＋ビジュアル|
|\<C-b\>|\<C-t\>|ジャンプした先から戻る|ノーマル＋ビジュアル|

# Quickrun(エディタ上からプログラムを実行)
|キー|デフォルト|機能|モード|
|:---:|:---:|:---:|:---:|
|rn|:Quickrun |プログラムを実行|ノーマル|
|\<C-c\>||Quickrunを停止|ノーマル|

# Git連携
|キー|デフォルト|機能|モード|
|:---:|:---:|:---:|:---:|
|st|:Gstatus\<Cr\>|git status|ノーマル|
|ad|:Gwrite\<Cr\>|git add|ノーマル|
|cm|:Gcommit\<Cr\>|git commit|ノーマル|
|co|:Gread\<Cr\>|git checkout|ノーマル|
|bm|:Gblame\<Cr\>|git blame|ノーマル|
|df|:Gdiff\<Cr\>|git diff|ノーマル|
|ps|:Git push|git push|ノーマル|

# その他キーマップ
|キー|デフォルト|機能|モード|
|:---:|:---:|:---:|:---:|
|;|:|コマンドモードへ入る|ノーマル＋ビジュアル|
|w|:w\<C-r\>|開いているバッファを上書き保存する|ノーマル|
|q|:q\<Cr\>|開いているバッファを終了する|ノーマル|
|qq|:qa\<Cr\>|全てのバッファを終了する|ノーマル|
|<C-/><C-/>|:TComment\<Cr\>|選択行をコメントアウトする|ノーマル＋ビジュアル|
|\<Esc\>\<Esc\>|:\<C-u\>nohlsearch\<Cr\>\<Esc\>|ハイライト表示を解除|ノーマル＋ビジュアル|
|\<C-a\>|^|行の先頭へ移動|ノーマル＋ビジュアル|
|\<C-e\>|$|行の末尾へ移動|ノーマル＋ビジュアル|
|s|:%s/|置換|ノーマル＋ビジュアル|
|vs|:\<C-u\>imShellPop\<Cr\>|VimShellが起動|ノーマル＋ビジュアル|

# 特殊キー対応表
|表記|キー|意味|
|:---:|:---:|:---:|
|\<C-x\>|Ctrl+x|Controlキーと任意のキーの組み合わせ|
|\<S-x\>|Shift+x|Shiftキーと任意のキーの組み合わせ|
|\<Cr\>|Return|Enterキー|
|\<Esc\>|Esc|Escapeキー|
|\<Tab\>|Tab|Tabキー|

上記以外の特殊キーのコードが知りたい場合
```vim
:help keycodes@ja
```
で閲覧可能