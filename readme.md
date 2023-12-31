## FPGA project
### 組員
 - 111321019 資工二 熊芊瑀
 - 111321035 資工二 朱薔媚

### 遊玩玩法
#### 輸入介紹
![輸入](https://github.com/lazybear0425/FPGA-project-111321019-111321035/assets/155285032/276a61cb-ec38-4aa0-a0ca-5bba7692cd7a)
 - 左邊開關(紅色)
   - 用於操縱方向
   - 控制下上左右(依序)
 - 右邊開關(藍色)
   - 用於reset棋盤，跟確定放置區域
   - 2:reset(左邊數來第二個)
   - 4:確定放置區域
#### 棋盤
![遊玩畫面](https://github.com/lazybear0425/FPGA-project-111321019-111321035/assets/155285032/d617ba86-0447-4d7e-9235-bb5e8638839b)
 - 紅色燈為player 1，綠色燈為player 2，藍色燈為目前游標位置
 - player 1贏了畫面
 - ![player1_win](https://github.com/lazybear0425/FPGA-project-111321019-111321035/assets/155285032/dd60d08d-9780-4443-9ee4-eabae83f2c7d)
 - player 2贏了畫面
#### 顯示
![20231231_152805](https://github.com/lazybear0425/FPGA-project-111321019-111321035/assets/155285032/687fee44-f94b-48fe-b6e1-9d1c922e0c8e)
 - 用7段顯示器顯示
 - 一開始有99秒
   - 向下遞減，直到歸零
   - 歸零後，會**響動蜂鳴器**，代表犯規，**剩餘可犯規次數扣一**
 - 若剩餘可犯規次數歸零
   - 只剩60秒
   - 歸零後會響動蜂鳴器
#### LED
 - 紅色燈為player 1，綠色燈為player 2
 - D1~D3為player 1 剩餘可犯規次數
 - D7~D8為player 1是否贏了(開啟reset後才能知道)
 - D9~D11為player 2 剩餘可犯規次數
 - D15~D16為player 2是否贏了(開啟reset後才能知道)
### LCD輸出
![LCD](https://github.com/lazybear0425/FPGA-project-111321019-111321035/assets/155285032/b1bcb93c-795c-44bb-bd87-1cf3c7f47b7b)
