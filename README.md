# class23-09

## kata task1

[Task Link](https://www.codewars.com/kata/55d24f55d7dd296eb9000030)    
My solution    

    public class GrassHopper {

      public static int summation(int n) {
        int s=0;
        for (int i=0; i<=n; ++i){
            s=s+i;
        }
        return s;
      }
    }
My fav solution

    public class GrassHopper {

      public static int summation(int n) {

        return  n*(n+1)/2;
      }
    }
    
    
## kata task2

[Task Link](https://www.codewars.com/kata/542c0f198e077084c0000c2e)    
My solution

    public class FindDivisor {

        public long numberOfDivisors(int n) {
            int counter = 0;
            for (int i = 1; i <= n; ++i) {
                if (n % i == 0) {
                    counter++;
                }
            }
            return counter;
        }
    }
    
My fav solution

       import java.util.stream.IntStream;
        public class FindDivisor {
            public long numberOfDivisors(int n) {
            return IntStream.range(1, n+1).filter(i -> n%i==0).count();
            }
        }
