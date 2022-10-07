# for_5
模拟用户登录，有三次机会，三次未正确，则退出程序



//模拟用户登录场景，有三次机会，三次未正确，程序退出
int main()
{
	int i = 0;
	char password[20] = { 0 };//存起来
	for (i = 0; i < 3; i++)
	{
		printf("请输入密码：>");
		scanf("%s", password);
		if (strcmp(password, "123456") == 0)//不能比较两个字符串是否相等，应该使用库函数-strcmp
		{
			printf("登录成功\n");
			break;
		}
		else
		{
			printf("密码成功\n");
		}
	}
	if (i == 3)
		printf("三次密码均错误，退出程序\n");
	return 0;

}
