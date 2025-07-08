# How to naming for C++
@2025/06018

## 禁止事項
- アンダースコア始まりの命名

## ファイル名
- PascalCase.cpp/hpp
- １クラス１ファイルが目安

## クラス
- PascalCase
### メソッド
- PascalCase()
### メンバ
- 

## 構造体
常にメソッド・メンバが公開
- PascalCase_St

## 関数

### 終了・停止
#### 正常系
##### 終了する
- quite + 名詞 ： 〇〇をやめる
- exit ： やめる、出る
- close : 閉じる（ファイルやコネクト）
- finish/complete : やり遂げる
- end : 終わらせる
##### 取り消す
- cancel
##### 停止する
- stop ： 再開しうる
- pause ： 再開する前提
- terminate ： 再開しない
#### 異常系
##### 中止する
- abort
##### 強制終了する
- kill

## 変数
- snake_case
### 真偽値
#### 状態
is + 形容詞
- is_empty
- is_null
- is_changed
#### 完了
has + 過去分詞
- has_read
- has_written
- has_changed
#### 可能
can + 動詞
- can_read
- can_write
#### 要求
should + 動詞
- should_continue
- should_stop
#### 存在
exists + 名詞
- exists_errot
- exists_file

### 文字列
#### ファイル
- fname_... = "xxx.txt"
#### ディレクトリ
- dir_... = "work\\"
#### パス
- apath_... : 絶対パス (absolute path)
- rpath_... : 相対パス (relative path)

## 定数
- constexpr SNAKE_CASE
- const k_snake_kase

## 制御
``` cpp:if
処理分岐
if (loop_count == 0) {
  ...
} else if (loop_count > 5) {
  ...
} else {
  ...
}
```
#### switch
同階層の関数呼び出し分岐や列挙子による制御
``` cpp:switch
switch (command) {
  case 0:
    RunProccess1();
    break;
  case 1:
    RunProccess2();
    break;
  default:
    ; /* do nothing */
    break;
}
```
``` cpp:for
for (int i = 0; i < 3; i++) {
  if (i == 2) break;
}
```
``` cpp:while
int i = 0;
while (!should_stop) {
  i++;
  if (i == 2) break;
}
```
``` cpp:do-while
int i = 0;
do {
  i++;
  if (i == 2) break;
} while (!should_stop)
```
