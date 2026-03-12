C++11新特性
auto关键字：
- auto 关键词用来做自动类型推导，就是编译器会在编译期间==根据初始化的值自动推导出变量的类型==
- 使用格式：`auto 变量名 = 值;`
  - auto 本质上是一个占位符，程序编译时会被真正的类型所代替
- 注意事项：
  - 使用 auto 声明变量时必须马上初始化
示例1： 基础类型
void test1()
{
	auto a = 10;       
	auto b = 3.14;     
	auto c = 'c';      
	auto d = "hello world";

	cout << sizeof(a) << ' ' << a << ' ' << typeid(a).name() << endl;
	cout << sizeof(b) << ' ' << b << ' ' << typeid(b).name() << endl;
	cout << sizeof(c) << ' ' << c << ' ' << typeid(c).name() << endl;
	cout << sizeof(d) << ' ' << d << ' ' << typeid(d).name() << endl;
}
