# LET

- Git 
	- Code task mới
		Khi code 1 task mới bạn phải về nhánh Main, khi code xong hoặc hết ngày làm việc phải checkout sang 1 nhánh khác và push lên repo

	-	Convension: 
		- Branch: tag/username/task-title
			Ví dụ: task/locbh3010/create-header
			Tag: dựa vào loại task được giao, gồm: fix, task

		- Commit (Lưu ý mỗi branch sẽ chỉ có commit): 
			Khi tạo task xong thì commit là [tag][username]:task description
			Ví dụ: [task][locbh3010]:create header for auth layout, create header for global layout
			
		- Lưu ý: Mỗi branch sẽ chỉ có 1 commit, nếu hết ngày làm việc bạn commit và đã push lên, hôm sau khi làm tiếp công việc và commit thì dùng command sau
			git add .
			git commit --amend --no-edit

	- Hoàn thành task: 
		- Khi hoàn thành task thì bạn phải tạo pull request (merge request) và gửi kèm vào báo cáo ngày hôm đó
		- Khi có conflict sẽ tiến hành fix conflict theo bước sau:
			- 1: Kiểm tra nhánh hiện tại còn code change mà chưa thay đổi thì tiến hành commit
			- 2: Checkout về main và pull code mới nhất
			- 3: Checkout sang nhánh cần fix conflict
			- 4: git rebase origin/main 
			- 5: vào giao diện source control của vscode và tiến hành fix conflict các file trong Tab Merge Changes
			- 6: Khi fix xong conflict thì gõ command:
				git add .
				git rebase --continue
			- 7: push code
- Báo cáo công việc:
# 
Ngày ... tháng ... năm
# Công việc hôm nay
1. Tên công việc
	mô tả: 
	Tiến độ: 
	Link pull request (nếu có): 
\# Công việc ngày mai
 -- như trên
