# Bubble-Sort
Bubble Sort Ascending/Descending
public class BubbleSort {
        for(int i = 1; i < data.length; i++){
            for(int j = data.length-1; j >= 1; j--){
                if(data[j] < data[j-1]){
                    t = data[j];
                    data[j] = data[j-1];
                    data[j-1] = t;
                }
            }
        }
        return data;
    }
    public static int[] descending(int[] data){
        int t;
        for(int i = 1; i < data.length; i++){
            for(int j = data.length - 1; j >= 1; j--){
                if(data[j] > data[j-1]){
                    t = data[j];
                    data[j] = data[j-1];
                    data[j-1] = t;
                }
            }
        }
        return data;
    }
    public static void main(String[] args) {
         int[] number = new int [100];
        System.out.println("Before Sorting : ");
        for(int i = 0; i < 100; i++){
        number[i] = (int) (Math.random() * 101);
        System.out.println(number[i]);
        }
        int[] sort = ascending(number); //Input ascending / descending here !
        System.out.println("After Sorting : ");
        for(int i = 0; i < 100; i++){
            System.out.print(number[i] + " ");
        }
    }   
}
