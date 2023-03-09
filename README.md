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



package Matrix;

public class Q3 {
	public static int sum_biggest_num_each_line(int[][] m) {
		int sum = 0;
		int max = 0;
		for(int i = 0; i < m.length; i++) {
			sum += max;
			max = m[i][0];
			for(int j = 1; j < m[i].length; j++) {
				if(m[i][j] > max) {
					max = m[i][j];
				}
			}
		}
		return  sum / m.length;
	}
}





package Matrix;

public class Q4 {
	public static int sum_smallest_num_each_line_positive(int[][] m) {
		int counter = 0;
		int sum = 0;
		int min = 0;
		for(int i = 0; i < m.length; i++) {
			sum += min;
			min = m[i][0];
			for(int j = 1; j < m[i].length; j++) {
				if(m[i][j] > 0) {
					if(m[i][j] > min) {
						min = m[i][j];
					}
				}
			}
		}
		return  sum / counter;
	}
}

