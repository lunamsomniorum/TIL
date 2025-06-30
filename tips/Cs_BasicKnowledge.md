# Hello World
``` cs:HelloWorld.cs
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
 
namespace Sample101 {
    class Program {
        static void Main(string[] args) {
            //  コンソールにHelloWorldと表示して終了
            Console.WriteLine("HelloWorld.");
        }
    }
}
```
## usingディレクティブ
### [System](https://learn.microsoft.com/ja-jp/dotnet/api/system?view=net-8.0)
- 一般的に使用される値と参照データ型、イベントとイベント ハンドラー、インターフェイス、属性、および処理例外を定義する基本クラスと基底クラスが含まれています。

### [System.Collections.Generic](https://learn.microsoft.com/ja-jp/dotnet/api/system.collections.generic?view=net-9.0)
- ジェネリック コレクションを定義するインターフェイスとクラスが含まれています。
- これにより、ユーザーは、非ジェネリックの厳密に型指定されたコレクションよりも、型の安全性とパフォーマンスを向上させる厳密に型指定されたコレクションを作成できます。

### [System.Linq](https://learn.microsoft.com/ja-jp/dotnet/api/system.linq?view=net-9.0)
- 統合言語クエリ (LINQ) を使用するクエリをサポートするクラスとインターフェイスを提供します。
#### LINQとは
- コレクション(配列やList、Dictionaryなど)の要素を処理するメソッドを集めたライブラリ
- forやforeachの高機能版ともいえ、ループ処理を簡潔に記載できる点が大きなメリット
- データベースやXMLを操作する際にもよく使う
  - 処理をメソッドで指定できる
  - IEnumerable型に実装されており、IEnumerable型を返す
  - LINQの処理は遅延実行される

### [System.Text](https://learn.microsoft.com/ja-jp/dotnet/api/system.text?view=net-8.0)
- ASCII および Unicode 文字エンコーディングを表すクラス (バイトのブロック間で文字ブロックを変換するための抽象型基本クラス、String の中間インスタンスを作成せずに String オブジェクトを操作および書式設定するヘルパー クラス) が含まれています。

### [System.Threading.Tasks](https://learn.microsoft.com/ja-jp/dotnet/api/system.threading.tasks.task?view=net-8.0)
- 同時実行コードと非同期コードの記述作業を簡略化する型を提供します。
- 主な型は、待機および取り消し可能な非同期操作を表す Task と、値を返すことができるタスクである Task<TResult>です。
- TaskFactory クラスはタスクを作成および開始するための静的メソッドを提供し、TaskScheduler クラスは既定のスレッド スケジュール インフラストラクチャを提供します。


https://zenn.dev/inuinu/articles/40d3a9825c19de#%E5%85%A5%E9%96%80%E8%A8%98%E4%BA%8B%E3%82%84%E5%8B%95%E7%94%BB%E3%81%AF%E4%BF%A1%E7%94%A8%E3%81%A7%E3%81%8D%E3%81%AA%E3%81%84
https://blog.ecbeing.tech/entry/2022/03/03/100000
