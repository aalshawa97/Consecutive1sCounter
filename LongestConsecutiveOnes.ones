package SlicingQuestions;

import java.util.ArrayList;

public class LongestConsecutiveOnes {
	public static void main(String[] args) {
		int arr [] = {1, 1, 0, 1, 1, 0, 1, 0, 1, 1};
		int count = 0;
		//First convert the problem
		ArrayList<Integer> list = new ArrayList<Integer>();
		for(int i = 0; i < arr.length; i++) {
			//Count 1s
			if(arr[i] == 1) {
				count++;
				if(count > 0 && i == arr.length-1) {
					list.add(count);
				}
			}
			//Store 1s
			else {
				if(count > 0) {
					list.add(count);
				}
				list.add(arr[i]);
				count = 0;
				
			}
			
		}
		System.out.println(list);
		int maxSequence = 0;
		for(int i = 0; i < list.size(); i = i + 2) {
			int len = list.get(i);
			if((i+1) < list.size()) {
				len += 1;
			}
			if((i + 2) < list.size()) {
				len += list.get(i+2);
			}
			if(len > maxSequence) {
				maxSequence = len;
			}
		}
		System.out.println("max sequence: " + maxSequence);
	}

}
