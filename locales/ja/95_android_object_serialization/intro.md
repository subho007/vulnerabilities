
通信の利便性のためにオブジェクトをシリアル化したり、後で使用するためにオブジェクトを保存することはよくあります。 ただし、逆シリアル化されたデータまたはコードは、暗号化を使用して保護しない場合は、提供されたアクセサ関数を使用せずに変更することができます。 さらに、暗号化は依然としてクライアント側のセキュリティであり危険なセキュリティの前提です。

一時的なフィールドを含むクラスをシリアル化したのち、逆シリアル化しようとすると、非一時的なデータがある箇所が NULL になります。 これは、時間、環境ベースの変数、または重要な変数が持ち越されて不適切に使用されるのを防ぐ優れた方法です。

