# reversearray
public class Reversearray {
	/* Function to reverse arr[] from start to end*/
	static void reversearray(int arr[], int start, int end) {
		int temp;
		if (start >= end)
			return;
		temp =arr[start];
		arr[start]=arr[end];
		arr[end] =temp;
		reversearray(arr, start+1, end-1);
	}
	/* Utility that prints out an array on a line */
 static void printarray(int arr[], int size	) {
	 for ( int i =0; i < size; i++)
		 System.out.print(arr[i] +"");
	 System.out.println("");
 }
 /*Driver function to check for above functions*/
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int arr[]= {1,2,3,4,5,6};
		printarray(arr,6);
		reversearray(arr,0,5);
		System.out.println("reverse array is:");
	
				printarray(arr,6);	

	}

}
// contributor Desh Limbu 
