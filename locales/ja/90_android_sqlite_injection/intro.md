
Androidアプリには多くのユーザー情報が含まれています。
ユーザー名、パスワード、電子メールID、銀行詳細などの機密情報が含まれます。この情報は、さまざまなテーブルを使用してSQLiteデータベースにアプリケーションによって格納されます。
それらを安全に保つために、アプリは安全かつ暗号化された形式で情報を保持することが求められます。

アプリケーションがデータベースを作成するたびに、デフォルトでは 
`/ data / data / app name / database /`  に保存されます。
この場所はアプリケーション専用の場所で、ユーザーや他のアプリからはアクセスできません。 SQLiteデータベースに保存されたデータを共有するために、アプリはコンテンツプロバイダを使用できます。

ただし、これらのデータベースには暗号化のための組み込みサポートはないため、これらのファイルにはすべての情報がプレーンテキスト形式で保存されます。
