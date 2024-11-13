Longest Substring Without Repeating Characters
Given a string s, find the length of the longest substring without repeating characters.

------------------------------------

//is char present in substr?
//-> yes : then s1.substring(s1.indexOf(s.charAt(i))) then add char to s1
//-> no  : add char to s1 and check for max length
class Solution {
    public int lengthOfLongestSubstring(String s) {
        int max=0;
        String s1="";
        for(int i=0;i<s.length();i++)
        {
            if(s1.contains(Character.toString(s.charAt(i))))
            {
                s1=s1.substring((s1.indexOf(s.charAt(i)))+1);
                s1=s1+s.charAt(i);
            }
            else
            {
                s1=s1+s.charAt(i);
                if(s1.length()>max)//checks max length
                {
                    max=s1.length();
                }
                 
            }
            //
        }
        return max;
    }
}
