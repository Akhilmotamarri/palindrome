# palindrome
java
class Solution {
    public boolean isPalindrome(int x) {
        if(x==0) return true;
        if(x<0 || x%10==0) return false;
        
        int t=x;
        int rev=0;
        while(t!=0){
            int r=t%10;
            t/=10;
            rev=rev*10+r;
            
        }
        if(x==rev) return true;
        else return false;
        
    }
}
