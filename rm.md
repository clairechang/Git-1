# RM

> git rm 用來刪除檔案庫中的檔案, 也可以刪除檔案

	git rm --cached filename 檔案庫還沒有加入過使用(表示沒有執行過 git commit)
	git rest HEAD filename 檔案庫已經有檔案了
	git rm 刪除檔案條件
		Git 索引中有沒有該檔案(執行過git add) 若有則不成立, 放棄
		檔案和Repo裡的內容是否一樣, 不一樣則不成立, 放棄
		
> 小技巧：刪除實體檔案和Repo裡的檔案

> 手動刪除實體檔案

	git add -A (會把不存在的檔案記錄在索引中)
	git commit (從 Repo 刪除檔案)