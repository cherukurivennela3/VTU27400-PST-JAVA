class Solution {
    public boolean halvesAreAlike(String s) {
    int mid = s.length()/2;
    int CountA = 0, CountB = 0;
    for(int i=0;i<s.length();i++){
        char ch = s.charAt(i);
        if (isVowel(ch)){
            if(i < mid)
              CountA++;
            else 
              CountB++;
        }
    }  
    return CountA == CountB ;     
    }
    private boolean isVowel(char c) {
        return "aeiouAEIOU".indexOf(c) != -1;
    }
}
