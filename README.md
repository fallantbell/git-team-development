# git-team-development  
## 圖解git 團隊開發流程  
### 先到想要合作的專案(這裡使用new-repo) 點擊右上角的fork 這樣就會將專案複製一分到自己的github上
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20130054.png)  
### 新增一個資料夾  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20130200.png)  
### 打開cmd 進入資料夾並使用git init 初始化  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20130239.png)  
### 點擊專案右上角綠色的code 並複製網址  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20130313.png)  
### 回到cmd 使用git clone 網址 將專案下載到本地端  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20130335.png)  
### 可以看到有一個新的資料夾 new-repo  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20130401.png)  
### 裡面有一個readme 代表成功下載  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20130412.png)  
### 使用git remote -v 的指令 可以看到origin 這代表連結到自己的github上  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20130445.png)  
### 但是為了要同步資料 我們還需要連結到原本fork的專案  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20130624.png)  
### 回到原本fork的專案 一樣點擊綠色的code 複製網址  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20130647.png)  
### 使用git remote add upstream(名稱可以自取) 網址  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20130717.png)  
### 再次使用 git remote -v 可以發現連到原本fork的專案  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20130731.png)  
### 假設今天我修改了專案的內容  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20131506.png)  
### 首先需要使用 git add . 將修改的內容存入暫存區  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20131533.png)  
### 接著使用git commit 的指令 將這些變更加上註解  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20131544.png)  
### 進入vim 使用i來進入insert 模式  
### 第一行黃色的字代表commit 標題    
### 第二行以後紅色的字就是commmit內容  
### 加完註解就使用 esc 然後 :x 退出  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20131633.png)  
### 之後使用git push origin(自己的github) main(想要push的分支) 指令將電腦上修改完的資料同步到github上  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20131722.png)  
### 修改成功 接者要將我們修改的資料同步到我們原本fork的專案  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20131948.png)  
### 按下pull request(簡稱 pr)  
### 可以看到修改的內容 還有我們要從自己的哪個分支推送到專案的哪個分支  
### 確認沒問題就按下create pull request  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20132040.png)  
### 查看commit內容 發送pr  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20132055.png)  
### 接者專案負責人就會看到 pr  
![image](https://github.com/fallantbell/git-team-development/blob/main/186476170_207966067836726_2543497359209531814_n.png)  
![image](https://github.com/fallantbell/git-team-development/blob/main/185269375_195204065673179_202858041547604476_n.png)  
### 點擊commit可以查看 pr的詳細內容  
![image](https://github.com/fallantbell/git-team-development/blob/main/187306164_141838484600091_7103733750045696123_n.png)  
### 可以看到做了那些更動  
![image](https://github.com/fallantbell/git-team-development/blob/main/188535066_906314969930888_7291472237687673683_n.png)  
### 負責人確認沒問題就可以把pr 合併  
![image](https://github.com/fallantbell/git-team-development/blob/main/186482571_489127809038762_4773239112638924196_n.png)  
### 可以看到成功的更新  
![image](https://github.com/fallantbell/git-team-development/blob/main/186173527_306772867575949_6482346818256527441_n.png)  
### 如果別人更新了專案資料 要怎麼同步到自己的電腦上呢?  
### 那就會用到一開始設定的upstream(代表合作的專案)  
### 使用git pull upstream main(想要pull的分支) 這樣就會將遠端的資料下載下來並且合併  
### 如果想要同步到自己的github上面 就一樣使用add commit 指令  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20133112.png)  
### 最後再push 回去就可以了  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20133159.png)  

