# hello-world
public class Main {
	
	public static boolean isSorted(int[] array, int lenght) {
		if(array == null || lenght<2) {
			return true;
		}
		if(array[lenght-2]>array[lenght-1]) {
			return false;
		}
		return isSorted(array,lenght-1);
	}

	public static void main(String[] args) {
		
		int[] array = {0,1,4,7,1};
		boolean b = isSorted(array, array.length);
		System.out.println(b);
