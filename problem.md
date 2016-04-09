gitbash使用中的一些常见问题
1.git pull的时候弹出另一个界面：
 # Please enter a commit message to explain why this merge is necessary.
        如果需要的话请输入一个提交信息来说明你这此合并。
解决方法：这个界面是在pull服务器代码和你本地代码做合并的时候，让你填写合并信息的。你可以不用管。如果公司有固定的提交格式的时候你就需要：
按键盘上字母i，进入insert模式去修改最上边一行合并信息。然后在输入冒号+wq保存退出即可。
             如果合并信息没有强制要求格式，有以下几种办法：
             1.输入：wq注意是冒号+wq，直接保存退出
             2.输入：q就是直接退出
             3.在键盘上按ctrl + z(强制退出)
2.弹出错误：
  fatal: ... does not appear to be a git repository
  fatal: Could not read from remote repository.
  Please make sure you have the correct access rights and the repository exists.
解决方法：
	修改 .git 下的 config 文件，修改url的内容。