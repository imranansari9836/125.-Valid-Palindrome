class Solution {
    public boolean isPalindrome(String s) {
       String tempString = s.replaceAll("[^A-Za-z0-9]", "").toLowerCase();
        // Reverse the tempString 
        String rev = new StringBuffer(tempString).reverse().toString();
        // check tempString to rev String 
        return tempString.equals(rev);
    }
}
