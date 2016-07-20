# ReverseWordsinString
import java.util.Scanner;

public class ReverseWords {

	public static void main(String[] args) {
		Scanner cc=new Scanner(System.in);
		System.out.println("Enter the String");
		String s = cc.nextLine();

		String q[] = s.split(" ");
		StringBuffer y[] = new StringBuffer[q.length];
		for (int i = 0; i < q.length; i++) {
			y[i] = new StringBuffer(q[i]);
		}
		StringBuffer qq = new StringBuffer();
		for (int i = q.length-1; i >=0; i--) {
			qq = qq.append(y[i]+ " ");
		}
		System.out.println("output String:");
		System.out.println(qq);
	}

}
