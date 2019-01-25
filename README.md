# Employee-Hours-Worked
#Python
	
	public class ComputeEmployeeWeeklyHoursClass {


	public static void main(String[] args) {
		// Employee's weekly hours
		int[][] hours = {
				{2, 4, 3, 4, 5, 8, 8},
				{7, 3, 4, 3, 3, 4, 4},
				{3, 3, 4, 3, 3, 2, 2},
				{9, 3, 4, 7, 3, 4, 1},
				{3, 5, 4, 3, 6, 3, 8},
				{3, 4, 4, 6, 3, 4, 4},
				{3, 7, 4, 8, 3, 8, 4},
				{6, 3, 5, 9, 2, 7, 9}};
		
		for (int i = 0; i < hours.length; i++) {
			int sum = totalHours(hours, i);
			System.out.println("Employee " + i + ": " + sum);
		}
	}

	public static int totalHours(int[][] time, int rowIndex) {
		
		int total = 0;
		int i = 0;
		for (int column = 0; column < time[i].length; column++) {
			total += time[rowIndex][column];
		}
	return total;
	} 
	}
