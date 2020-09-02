# 前提
[初回の設定](https://gitlab.com/hackathon_lite_SKFRONT/sandbox/-/wikis/Git+Docker-%E5%85%A8%E5%93%A1%E5%90%91%E3%81%91/1.%E5%88%9D%E5%9B%9E%E3%81%AE%E8%A8%AD%E5%AE%9A)の手順に従い、sshキーが配置されているという前提で進みます

# コマンド

dockerのターミナルや、git-bash、TeraTermを用いて、以下コマンド

（カレントはどこでも大丈夫です）

`ssh -i ~/.ssh/mimamoru-key.pem ec2-user@ec2-54-150-120-136.ap-northeast-1.compute.amazonaws.com`

![2020-09-02](uploads/4af33aa885bd2294ef72cdc6ad894877/2020-09-02.png)

以上