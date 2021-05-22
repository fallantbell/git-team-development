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
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20132005.png)  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20132722.png)  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20132752.png)  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20133112.png)  
![image](https://github.com/fallantbell/git-team-development/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-05-22%20133159.png)  

