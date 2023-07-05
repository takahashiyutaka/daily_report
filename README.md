# 使用方法 
## 管理者  
1. このリポジトリに研修生のGitHubアカウントを招待する  
    Setting->Collaborators->Add people->研修生GitHubアカウントのEmailを記入  
## 研修生  
1. リモートリポジトリをローカルリポジトリにクローン  
    ```zsh  
    // リポジトリのクローン  
    1-1. git clone $url  

    // ブランチの作成(アッパーキャメルケース)  
    1-2. git switch -c $MyName  

    // READMEファイルの名前変更  
    1-3. mv README.md $MyName.md
    ```  
2. **日報用テンプレート**(下記に記載あり)を使用し日報を記入  
3. 自身のローカルリポジトリからリモートリポジトリにpush
    ```zsh  
    // ステージング
    3-1. git add $MyName.md

    // コミット
    3-2. git commit -m '日報：$MyName'

    //プッシュ
    3-3. git push origin $branch(1-2で作成したブランチ)
    ```
4. リモートリポジトリで自身のブランチからmergeブランチへpullrequest  
5. merge  
## 注意事項
- ### .githubディレクトリは変更しないでください。  

# 日報用テンプレート(コピーして使用してください)
```*.md
## :名前  
- ⚪︎月⚪︎日(⚪︎)  
## 【進捗に関して】  
- example  
## 【取組詳細】  
> - example  
## 【次回の目標】  
- example  
## 【その他相談したいこと】  
- example