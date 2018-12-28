# fork_test
* githubのfork, pull requestの練習用

## 手順 Fork, localにclone後
1. 作業ブランチ(topic)を作成，作業
1. リモート(origin)にpush
1. 必要なら作業を続ける
1. プルリクを送る段階になったら，fork元のリポジトリをリモートとして追加(upstream)，add remote，その後fetch
1. originのmasterをupstreamのmasterに進める，merge (前と合わせてpullでもよい)
1. topicブランチを最新のmasterからの履歴に変更， rebase
1. topicを無理やりoriginにpush, push -f
1. GitHubのoriginページからupstream側にpull requestを送る

## 手順 マージ側
1. pull requestをくれたユーザをリモートとして追加
1. ローカルでブランチを切って試す
1. 不備がなければmasterにマージしてpush
1. リモートの登録を解除， remote rm

## 参考ページ
* https://qiita.com/tsuruokax/items/aa720561ee4f078bda60
* https://numb86-tech.hatenablog.com/entry/2017/02/25/143908

* http://5509.hatenablog.com/entry/2012/03/13/164234
* https://qiita.com/ngtkk/items/05097d127db6a415a7d8

# 複数githubアカウントを使う方法
* sshが同じキーならそれが登録されているアカウントでログインしたことになる
* ので別のキーを作って別のアカウントにはそのキーを登録した

## 参考ページ
* https://stackoverflow.com/questions/40069344/remote-rejected-master-master-permission-denied
* https://qiita.com/fantasista_21jp/items/bff8157efbacc9355dbe
