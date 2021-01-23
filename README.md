# 關於 分支
本Repo會遵循Git-flow的模式來做管理。透過這種開發模式來確保最終成品的出錯率是很低的狀態。以下會說明本Repo會有的分支。  
***
以下是必定會有的：  
1. master：正式對外發布的版本，不能做任何修改，只能由管理者從release做匯入。  
2. hotfix：master版本發布時如出現重大問題，會透過加開hotfix分支，而這個分支是臨時的，完成後會匯到master和develop。  
3. release：測試版本，是master發布前的最終檢查和檢測，不能做任何修改，只能由管理者從develop做匯入。  
4. develop：開發版本，是開發時主要操作的分支，會接收各個開發人分支的匯入，也會接收release的匯入(有Bug時)、hotfix的匯入。  
5. \<UserName\>\_develop：開發人內部開發版本，是每個開發人在上傳到develop的前置匯集分支，只能由該開發人或管理者進行操作。  
  
以下是可能會有的：
1. \<UserName\>\_func\_<FunctionName>：開發人內部開發的功能分支，是開發各個功能時可能創建的分支，這個分支只能匯出到\<UserName\>\_develop做整合。  
2. \<UserName\>\_temp：開發人內部開發的暫存分支，是用來暫存非該階段工作事項的暫存分支，通常會搭配stash命令座使用。
