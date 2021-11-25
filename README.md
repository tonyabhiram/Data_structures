import java.util.Scanner;
public class Main {
	public static void main(String[] args) {
		Scanner in = new Scanner(System.in);
		int n=in.nextInt();
		int i,j,c=0;
		int[] a= new int[n];  
		for(i=0;i<n;i++){
		    a[i]=in.nextInt();  
		}
		for(i=0;i<n;i++){
			for(j=0;j<n;j++){
				    if(a[i]==a[j]){
				        c=c+1;
				    }
			}
			
		}
	
		if(c-n==0){
			System.out.println("No Duplicates are present");
		}
		else{
			System.out.println("Duplicates Found");
		}
}
}
