# -
个人学习
package one;

public class Demo1 {
	public static void main(String[] args) {
		float r = 6400 * 1000;
		float c = 2 * 3.14f * r;
		float v = 9.8f;
		float second = c / v;
		float day = second / 3600 / 24;
		System.out.println("跑赤道一圈要" + day + "天");
//        强制整数，直接去掉小数部分
		int day1 = (int) day;
		System.out.println("跑赤道一圈要" + day1 + "天");
//		上取整数，结果是double
		double day2 = Math.ceil(day);
		int day3 = (int) day2;
		System.out.println("跑赤道一圈要" + day2 + "天");
		System.out.println("跑赤道一圈要" + day3 + "天");
//		下取整数，结果为double47.0
		double day4 = Math.floor(day);
		System.out.println("跑赤道一圈要" + day4 + "天");

		char a = '中';
		char b = 'a';
		char c1 = '\u4ba5';// \转义字符
		float pi = 3.14f;
//		final定义常量，常量大写
		final float PI = 3.14f;
		System.out.println(PI * 300);
//		字符可以当成整数用，用它的ASCII值参与运算
//		算术运算
		System.out.println(0 + 'a');
//		字符串连接“0”+“a”
		System.out.println(0 + "a");

		String a2 = "春来江水绿如蓝\t";
		String b2 = "System.out.println(\"输入圆半径：\");\n";
		String c2 = "能不忆江南？\t";
		char d2 = '\'';
		System.out.println(a2);
		System.out.println(b2);
		System.out.println(c2);
		System.out.println(d2);

		boolean f = true;
		Boolean g = f;// 装箱
		boolean h = g;// 拆箱

		String i = "asadsaf";
		String j = "12345";
		// 类.函数(字符串参数)=>整数
		// 函数相当于一个加工厂，参数是原料，返回值是它的产品
		// 字符串转整数
		int k = Integer.parseInt(j);
		int m = Integer.valueOf(j);

		int n = 'A';
		// 整数常量->char;
		char o = 65;
		System.out.println("\n" + o);
		int q = 12;
		char p = (char) q;
//		把字符当成整数使用，取ASCII值;
		System.out.println("a~z共有" + ('z' - 'a' + 1));

//		四舍五入
		double rr = Math.rint(3.54 + 0.5);
		System.out.println(rr);

		int s = (int) (3.54 + 0.5);
		System.out.println(s);

		/*
		 * 学号：21120132 成绩1：98.5 成绩2：94.0 成绩3：78.5 性别：f 是否理科:true 班级排名：5
		 */
		String studentId = "21120132";
		float score1 = 98.5f;
		float score2 = 94.0f;
		float score3 = 78.5f;
		char sex = '男';
		boolean isScience = true;
		int rank = 1;
		System.out.println("学号：" + studentId);
		System.out.println("成绩1：" + score1);
		System.out.println("成绩1：" + score2);
		System.out.println("成绩1：" + score3);
		System.out.println("性别：" + sex);
		System.out.println("是否理科：" + isScience);
		System.out.println("班级排名：" + rank);
	}

}
import java.util.Scanner;
public class Main{
	public static void main(String[] args){
		System.out.println("开始");
Scanner sc = new Scanner(System.in);
System.out.println("请输入一个星期数(1-7):");
int week = sc.nextInt();
switch(week){
	case 1:
		System.out.println("星期一");
		break;
	case 2:
		System.out.println("星期二");
		break;
	case 3:
		System.out.println("星期三");
		break;
	case 4:
		System.out.println("星期四");
		break;
	case 5:
		System.out.println("星期五");
		break;
	case 6:
		System.out.println("星期六");
		break;
	case 7:
		System.out.println("星期日");
		break;
	default:
		System.out.println("你输入的星期数有误");
		break;
}

	
	}
}
