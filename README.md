import java.util.Scanner;
public class PrimeSum{
public static void main(String[] args){
Scanner sc=new Scanner(System.in);
int n=sc.nextInt();
int sum=0;

int arr[]=new int[n];
for(int i=0;i<n;i++){
arr[i]=sc.nextInt();
}
for(int i=0;i<n;i++){
int count=0;
	for(int j=1;j<=arr[i];j++){
	if(arr[i]%j==0)
	count++;
	}
if(count==2){
sum=sum+arr[i];
}
}
System.out.println(sum);
}
}
