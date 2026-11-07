---
title: JTBG洛谷团队加入要求
date: 2026-11-07 19:56:54
tags:
---
# 加入要求

请运行 以下程序:  
<!-- more -->
```cpp
#include <bits/stdc++.h>

#ifdef USE_JTBG_H
	#undef JTBG_ALL
	#undef _agree_
	#define JTBG_ALL
	#undef _agree_
	#include "jtbg.h"
#endif

#define please return
#define AC 0

using namespace std;
int main()
{
	double s = 0.0;
	cout << "请输入用户名:";
	string usrn;
	getline(cin, usrn);
	if (usrn == "_guitu_") s += 100.0;
	if (usrn == "kkksc03") s += 10000.0;
	cout << "请输入TAG(无记为\"none\"):";
	string tag;
	getline(cin, tag);
	if (tag == "作弊者") s -= 50.0;
	else if (tag != "none") s += 50.0;
	cout << "wait..." << endl;
	cout << "[1] gray" << endl;
	cout << "[2] blue" << endl;
	cout << "[3] green" << endl;
	cout << "[4] orange" << endl;
	cout << "[5] red" << endl;
	cout << "[6] purpule" << endl;
	cout << "请输入名字颜色:";
	int col;
	cin >> col;
	if (col == 1) s += 10.0;
	if (col == 2) s += 20.0;
	if (col == 3) s += 30.0;
	if (col == 4) s += 50.0;
	if (col == 5) s += 75.0;
	if (col == 6) s += 100.0;
	double test = 0.0;
	int a, b, c, d, e, f, g, h, i;
	cin >> a >> b >> c >> d >> e >> f >> g >> h >> i;
	test = (a * 1.0 + b * 2.0 + c * 5.0 + d * 10.0 + e * 15.0 + f * 20.0 + g * 30.0 + h * 50.0 + i * 100.0) / 3.1;
	s += test;
	cout << "成绩单" << endl;
	cout << usrn << "[" << tag << "]" << endl;
	cout << "成绩:" << s << endl;
	cout << "结果:";
	if(s<50.0) cout<<"再接再厉"<<endl;
	else if(s<100.0)
	{
		cout<<"还不错"<<endl;
		cout<<"请前往\"https://www.luogu.com.cn/team/134157#join\"加入"<<endl;
	}
	else
	{
		cout<<"完美"<<endl;
		cout<<"请前往\"https://www.luogu.com.cn/team/134157#join\"加入"<<endl;
	}
	please AC;
}
```