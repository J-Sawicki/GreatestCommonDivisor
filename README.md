//# GreatestCommonDivisor
//Program that quickly checks for a greatest common divisor

public class GreatestCommonDivisor {
    public static int getGreatestCommonDivisor (int first, int second){
        if (first < 10 || second < 10 ){
            return -1;
        }
            for ( int i = (first>second) ? second : first; i>1; i--){
                if (first % i == 0 && second % i == 0){
                    System.out.println(i);
                    return i;
                }
            }
        return 1;
    }
}
