import java.util.Scanner;

public class Pattern {

	public static void main(String[] args) {
		
		Scanner in=new Scanner(System.in);
		int i,n,j,temp1,temp2;
		n=in.nextInt();
		temp1=n;
		for(i=0;i<n;i++)
		{
			for (j=(n);j>i;j--)
				System.out.print("\t");
		
			for(j=i;j>=0;j--)
			{
				if(j%2!=0)
				{
					temp1=1+j*n-(j-1)*j/2+i-j;
					System.out.print(temp1+"\t");					
				}
				else 
				{
					temp2=1+j*n-(j-1)*j/2+n-1-i;
					System.out.print(temp2+"\t");					
				}		
			}					
			System.out.println();	
		}

	}

}
