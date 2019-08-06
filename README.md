//ZeroAlgorithim

import java.io.*;
import static java.lang.Math.max;
import static java.lang.Integer.min;
import static java.lang.Math.abs;
import static java.lang.Math.pow;
import static java.lang.System.out;
import java.util.*;
public class Kaudo { 
    //Search about the number or the most number near and max
    static int max10[], max100[], max1000[];
    static int element[], min10[], min100[],min1000[];
    public static void main(String[] args)throws IOException
    {int n=100000,maxnumber=10000;//The maxnumber in array 10^4
    max10=new int[maxnumber/10+1]; max100=new int[maxnumber/100+1];max1000=new int[maxnumber/1000+1];
    //this array we can store the max number
    min10=new int[maxnumber/10+1]; min100=new int[maxnumber/100+1]; min1000=new int[maxnumber/1000+1];
    //this array we can store the min number
    element=new int[10001];
    for(int i=0;i<n;i++){
    int x=0;
    //Enter the Value of x
    if(max10[x/10]<x)max10[x/10]=x;
    if(min10[x/10]>x||min10[x/10]==0)min10[x/10]=x;
    if(max100[x/100]<x)max100[x/100]=x;
    if(min100[x/100]>x||min100[x/100]==0)min100[x/100]=x;
    if(max1000[x/1000]<x)max1000[x/1000]=x;
    if(min1000[x/1000]>x||min1000[x/1000]==0)min1000[x/1000]=x;
    element[x]++;
    }
    int m=100000;//number of search operation
    for(int i=0;i<m;i++){
    int x=0;
    //Enter the Value of x
    if(element[x]>0){//is the element
        
    }
    else if(max10[x/10]>x){
        findin10(x);
        //search in element
        }
    else if(max100[x/100]>x){findin100(x/10);}
    else if(max1000[x/1000]>x){findin1000(x/100);}
    else if(maxnumber>x){findin10000(x/1000);}
    }
    }
    
    static int findin10000(int x){
    x++;
    if(min1000[x]>0){return min1000[x];}
    x++;
    if(min1000[x]>0){return min1000[x];}
    x++;
    if(min1000[x]>0){return min1000[x];}
    x++;
    if(min1000[x]>0){return min1000[x];}
    x++;
    if(min1000[x]>0){return min1000[x];}
    x++;
    if(min1000[x]>0){return min1000[x];}
    x++;
    if(min1000[x]>0){return min1000[x];}
    x++;
    if(min1000[x]>0){return min1000[x];}
    return 0;}
    
    static int findin1000(int x){
    x++;
    if(min100[x]>0){return min100[x];}
    x++;
    if(min100[x]>0){return min100[x];}
    x++;
    if(min100[x]>0){return min100[x];}
    x++;
    if(min100[x]>0){return min100[x];}
    x++;
    if(min100[x]>0){return min100[x];}
    x++;
    if(min100[x]>0){return min100[x];}
    x++;
    if(min100[x]>0){return min100[x];}
    x++;
    if(min100[x]>0){return min100[x];}
    return 0;}
    static int findin100(int x){
    x++;
    if(min10[x]>0){return min10[x];}
    x++;
    if(min10[x]>0){return min10[x];}
    x++;
    if(min10[x]>0){return min10[x];}
    x++;
    if(min10[x]>0){return min10[x];}
    x++;
    if(min10[x]>0){return min10[x];}
    x++;
    if(min10[x]>0){return min10[x];}
    x++;
    if(min10[x]>0){return min10[x];}
    x++;
    if(min10[x]>0){return min10[x];}
    return 0;}
    static int findin10(int x){
        x++;
        if(element[x]>0){return x;}
         x++;
        if(element[x]>0){return x;}
         x++;
        if(element[x]>0){return x;}
         x++;
        if(element[x]>0){return x;}
         x++;
        if(element[x]>0){return x;}
         x++;
        if(element[x]>0){return x;}
         x++;
        if(element[x]>0){return x;}
         x++;
        if(element[x]>0){return x;}
         x++;
        if(element[x]>0){return x;}
        return 0;
}
}
