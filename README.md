# matrix1
homework
package Matrix;

public class Q2 {
	public static int sum_positive(int[][] m) {
		int counter = 0;
		int sum = 0;
		for(int i = 0; i < m.length; i++) {
			for(int j = 0; j < m[i].length; j++) {
				if(m[i][j] > 0) {
					sum += m[i][j];
					counter++;
				}
			}
		}
		return  sum / counter;
	}
}
