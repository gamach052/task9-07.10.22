###  [Task 8kyu](https://www.codewars.com/kata/5ae62fcf252e66d44d00008e/train/java)

Complete the function that calculates the area of the red square, when the length of the circular arc A is given as the input. Return the result rounded to two decimals.
### My solution
```Java
public class Kata
{
    public static int expressionsMatter(int a, int b, int c)
    {
        int d;
        int g;
        int h;
        int f;
        int k;
        int z;
        int q=0;
        d=a * (b + c);
        f=a * b * c;
        g=a + b * c ;
        h=(a + b) * c ;
        k=a*b+c;
        z=a+b+c;
        if(f>=d && f>=g && f>=h && f>=k && f>=z){
            q=f;
        }
        if(z>=f && z>=g && z>=h && z>=k && z>=d){
            q=z;
        }
        if(g>=f && g>=d && g>=h && g>=k && g>=z){
            q=g;
        }
        if(h>=f && h>=g && h>=d && h>=k && h>=z){
            q=h;}
        if(k>=f && k>=g && k>=h && k>=d && k>=z){
            q=k;}
        if(d>=f && d>=g && d>=h && d>=k && d>=z){
            q=d;}   return q;} }
```

### Fav solution

```Java
public class Kata
{
    public static int expressionsMatter(int a, int b, int c)
    {
        return  Math.max(Math.max(a + b + c, a * b * c),Math.max ((a + b) * c, a * (b + c)));
    }
}
 

```
I like this solution because I like it
