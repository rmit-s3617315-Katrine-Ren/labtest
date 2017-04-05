# labtest
 //gameAthlete 存放这局比赛参赛运动员信息的数组
	//selectedAthlete 存放符合比赛条件的运动员的数组
	
	public a //gameAthlete 存放这局比赛参赛运动员信息的数组
	//selectedAthlete 存放符合比赛条件的运动员的数组
	
	public athlete[] randomChoose(athlete[] selectedAthlete,athlete[] gameAthlete,int numberAthlete){
		int index;//随机在所有运动员数组中取得运动员的号码
		int length=TotalAthlete;
		int[] num=new int[length];
		for(int i=0;i<length;i++){
			num[i]=i;
		}
		for(int i=0;i<numberAthlete;i++){
			index=(int)(Math.random()*(length-1));//随机在所有运动员数组中取得运动员的号码
			randomPlayer[i]=selectedAthlete[num[index]];
			num[index]=num[length-1];
			length--;
		}
		return gameAthlete;
	}
