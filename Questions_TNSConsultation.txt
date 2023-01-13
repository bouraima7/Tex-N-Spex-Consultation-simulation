package Tutorial;

public class Questions {
	public String level;
	private String low = "beginner";
	private String med = "proficient";
	private String high = "advanced";
	
	public Questions(String level){
		this.level = level;
		
	}
	public void analyze() {
		if (this.level.equals(low)) {
			System.out.println("Ok, you're a beginner. No worries! We will get you to the profficient level very soon!");
		}
		else if (this.level.equals(med)) {
			System.out.println("Ok, you're at the profficient level. We will sharpen your skills so that you become advanced!");
		}
		else {
			System.out.println("So, you're advanced! Our goal is to make you into an expert so that you may even instruct others eventually");
		}
	}
}
