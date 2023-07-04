# OstadJavaLoopAssignment
## Output:
--------Pattern One--------
1 
2 3 
4 5 6 

--------Pattern Two--------
    1 
  2 3 
4 5 6 

--------Pattern Three--------
1 2 3 
4 5 
6 

--------Pattern Four--------
1 2 3 
  4 5 
    6 

--------Pattern Five--------
    1 
  2 3 4 
5 6 7 8 9 

## Code:
// pattern 1
	public void loopPatternOne() {
		int counter = 1;
		for (int i = 1; i <= 3; i++) {
			for (int j = 1; j <= i; j++) {
				System.out.print(counter + " ");
				counter++;
			}
			System.out.println();
		}
		System.out.println();
	}

	// pattern 2
	public void loopPatternTwo() {
		int counter = 1;
		int spacePrint = 4;
		for (int i = 1; i <= 3; i++) {
			for (int k = 1; k <= spacePrint; k++) {
				System.out.print(" ");
			}
			spacePrint -= 2;
			for (int j = 1; j <= i; j++) {
				System.out.print(counter + " ");
				counter++;
			}
			System.out.println();
		}
		System.out.println();
	}

	// pattern 3
	public void loopPatternThree() {
		int counter = 1;
		for (int i = 1; i <= 3; i++) {
			for (int j = 3; j >= i; j--) {
				System.out.print(counter + " ");
				counter++;
			}
			System.out.println();
		}
		System.out.println();
	}

	// pattern 4
	public void loopPatternFour() {
		int counter = 1;
		int spacePrint = 0;
		for (int i = 1; i <= 3; i++) {
			for (int k = 1; k <= spacePrint; k++) {
				System.out.print(" ");
			}
			spacePrint += 2;
			for (int j = 3; j >= i; j--) {
				System.out.print(counter + " ");
				counter++;
			}
			System.out.println();
		}
		System.out.println();
	}

	// pattern 5
	public void loopPatternFive() {
		int counter = 1;
		int spacePrint = 4;
		int flag = 1;
		for (int i = 1; i <= 3; i++) {
			for (int k = 1; k <= spacePrint; k++) {
				System.out.print(" ");
			}
			spacePrint -= 2;
			for (int j = 1; j <= flag; j++) {
				System.out.print(counter + " ");
				counter++;
			}
			System.out.println();
			flag += 2;
		}
		System.out.println();
	}



