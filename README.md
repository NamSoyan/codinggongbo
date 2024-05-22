package java0522;

public class Test9 {

	public static void main(String[] args) {
		/***********************************************
		 * 문제9) 2차원 배열를 이용하여 별(★)를 출력하시오
		 * 출력 예시)
	     *    ★
	     *   ★★★
	     *  ★★★★★
	     * ★★★★★★★
	     *  ★★★★★
	     *   ★★★
	     *    ★
		 ************************************************/

		// 해결 코드 작성 시작


	    String 별 = "★";
	
	    /*** 코드 시작 ***/
	    String[][] 배열 = new String[7][7];
	    String 빈공간 = " ";
	    
	    for(int i = 0; i < 배열.length; i++) {
	    	for(int j = 0; j < 배열[i].length; j++) {
	    		
		    		if((i == 0||i==6) && (j <= 2 || j >= 4 )) {
		    			배열[i][j] = 빈공간;
		    		} else if((i == 1||i==5) && (j <= 1 || j >= 5 )) {
		    			배열[i][j] = 빈공간;
		    		} else if((i == 2||i==4) && (j <= 0 || j >= 6 )) {
		    			배열[i][j] = 빈공간;
		    		} else if((i == 1||i==5) && (j <= 1 || j >= 5 )) {
		    			배열[i][j] = 빈공간;
		    		} else {
		    			배열[i][j] = 별;
		    		}
	    	}
	    }

		
	    for(int i = 0; i < 배열.length; i++) {
	    	for(int j = 0; j < 배열[i].length; j++) {
	    		System.out.print(배열[i][j]);
	    	}
	    	System.out.println();
	    }
	
	    /*** 코드 종료 ***/


	}

}



////////////////////////////////////////////////////////////////////////////////

package java0522;

public class Test8 {

	public static void main(String[] args) {

		/***********************************************
		 * 문제8) 2차원 배열를 이용하여 별(★)를 출력하시오
		 * 출력 예시)
	     * ★
	     * ★★
	     * ★★★
	     * ★★★★
	     * ★★★★★
	     * ★★★★
	     * ★★★
	     * ★★
	     * ★
		 ************************************************/

		// 해결 코드 작성 시작

	    String 별 = "★";
	
	    /*** 코드 시작 ***/
	    String[][] 배열 = new String[9][5];
	    
	    for(int i = 0; i < 배열.length; i++) {//행
	    	
	    	for(int j = 0; j < 배열[i].length; j++) {//열
	    		String 빈공간 = "";
	    	

    				  if((i==0||i ==8) && (j<=0)){
    					  배열[i][j] =별;
    			}else if((i==1||i ==7) && j<=1){
        				배열[i][j] =별;
        		 }else if((i==2||i ==6) && j<=2){
     					배열[i][j] =별;
        		 }else if((i==3||i ==5) && j<=3){
        			 	배열[i][j] =별;
        		 }else if((i==4||i ==4) && j<=4){
        			 	배열[i][j] =별;
        		 }else {
        			 	배열[i][j] ="";}

	    	
	    	}
	    	
	    }
	    
	    //출력 부분
		 for(int i = 0; i < 배열.length; i++) {
			    	
	    	for(int j = 0; j < 배열[i].length; j++) {
	    		System.out.print(배열[i][j]);
	    		
	    	}
    	System.out.println();
    	}
	    /*** 코드 종료 ***/

	}

}
