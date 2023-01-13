package Tutorial;
import java.util.Scanner;
import java.text.DecimalFormat;

public class main {
	
	private static final DecimalFormat df = new DecimalFormat("0.00");
	
	public static void main(String[] args) {
		Scanner input = new Scanner (System.in);
		
		
		System.out.println("Welcome to Tex N Spex LLC.");
		System.out.println();
		System.out.println("How may we help you? We offer the following services:");
		System.out.println();
		
		String[] services= {"JAVA","PYTHON","C++","WEB DEVELOPMENT","ENGLISH","FRENCH","SPANISH"};
		double [] prices = {30.00, 30.00, 25.00, 20.00, 15.00, 15.00, 15.00};
		for (int i=0; i<services.length; i++) {
			System.out.print(services[i]);
			System.out.println(" - $" + df.format(prices[i]));
		}
		
		String str;
		str= input.nextLine();
		str=str.toUpperCase();
		double total = 0;
		
		if (str.equals(services[0])){
			total = prices[0];
			System.out.println("Your total today is: "+ df.format(total));
		}
		else if (str.equals(services[1])) {
			total = prices[1];
			System.out.println("Your total today is: "+ df.format(total));
		}
		else if (str.equals(services[2])) {
			total = prices[2];
			System.out.println("Your total today is: "+ df.format(total));
		}
		else if (str.equals(services[3])) {
			total = prices[3];
			System.out.println("Your total today is: "+ df.format(total));
		}
		else if (str.equals(services[4])) {
			total = prices[4];
			System.out.println("Your total today is: "+ df.format(total));
		}
		else if (str.equals(services[5])) {
			total = prices[5];
			System.out.println("Your total today is: "+ df.format(total));
		}
		else if (str.equals(services[6])) {
			total = prices[6];
			System.out.println("Your total today is: "+ df.format(total));
		}
		
		System.out.println("Would you like any other service?");
		System.out.println();
		for (int i=0; i<services.length; i++) {
			System.out.print(services[i]);
			System.out.println(" - $" + prices[i]);
		}
		
		String str2= input.nextLine();
		str2=str2.toUpperCase();
		System.out.println();
		
		if (str2.equals(services[0])){
			total += prices[0];
			System.out.println("Your total today is: "+ df.format(total));
		}
		else if (str2.equals(services[1])) {
			total += prices[1];
			System.out.println("Your total today is: "+ df.format(total));
		}
		else if (str2.equals(services[2])) {
			total += prices[2];
			System.out.println("Your total today is: "+ df.format(total));
		}
		else if (str2.equals(services[3])) {
			total += prices[3];
			System.out.println("Your total today is: "+ df.format(total));
		}
		else if (str2.equals(services[4])) {
			total += prices[4];
			System.out.println("Your total today is: "+ df.format(total));
		}
		else if (str2.equals(services[5])) {
			total += prices[5];
			System.out.println("Your total today is: "+ df.format(total));
		}
		else if (str2.equals(services[6])) {
			total += prices[6];
			System.out.println("Your total today is: "+ df.format(total));
		}

		System.out.println("Before we get started, I would like to know your experience level.");
		System.out.println("Please input your experience level. It can be be beginner, proficient, or advanced.");
		
		System.out.println();
		String lvl = input.next();
		
		
		Questions que = new Questions(lvl);
		que.analyze();
	}
}
