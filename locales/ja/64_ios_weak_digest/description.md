
パスワードにソルトしたMD5を使用するのは避けてください。理由としては、暗号化の弱点ではなく速いためです。
攻撃者はシングルCPU上で毎秒数十億個の候補パスワードを試すことができます。

ファイルの整合性のためにMD5を使用することは、実際の使用シナリオに応じて、実際問題になったり、ならなかったりします。MD5に対する攻撃は、もし攻撃者が両方の攻撃をコントロールしている場合は、攻撃者が同じハッシュを持つ2つのファイルを作成するプリイメージ攻撃ではなく、衝突攻撃になります。
ただし、影響を受けていない既存のファイルのハッシュと一致することはできません。

SHA1はデータの整合性のためにGitとGnuPGで広く使われているハッシングアルゴリズムのままですが、
衝突攻撃の影響を受けやすいことも [証明](https://shattered.io/static/shattered.pdf)されています。