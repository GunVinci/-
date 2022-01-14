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

		int day1 = (int) day;
		System.out.println("跑赤道一圈要" + day1 + "天");
		
		double day2 = Math.ceil(day);
		int day3 = (int)day2;
		System.out.println("跑赤道一圈要" + day2 + "天");


	}

}
