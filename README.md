# BinarySearch in java
import java.util.*;
public class Arr{
public static int binarySearch(int numbers[], int key){
int start = 0;
int end = numbers.length-1;
while(start <= end){
int mid = (start+end)/2;
if(numbers[mid] == key){
return mid;
}
if(numbers[mid] < key){
start = mid-1;
}else{
end = mid-1;
}
}
return -1;
}
public static void main(String args[]){
int ar[] = {1,2,3,4,5,6,7,8};
int key = 4;
System.out.println(binarySearch(ar, key));
}
}


