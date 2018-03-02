# AmstrongNumber

  int numbers[][] = new int[1000][];
	int index = 0;
		
	for(int i = 0; i < 1000; i++) {
		numbers[i] = new int[]{ i/100, (i%100)/10, i%10 };
		if (Math.pow((double)numbers[i][0], 3) + 
				Math.pow((double)numbers[i][1], 3)+
				Math.pow((double)numbers[i][2], 3) 
				== i) {
			index++;
			System.out.printf("第%d個數字：%d%n",index, i );			
			
		}
	}
