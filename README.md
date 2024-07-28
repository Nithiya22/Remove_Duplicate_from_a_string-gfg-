# Remove_Duplicate_from_a_string-gfg-
class Solution {
    String removeDups(String str) {
        #use LinkedHashSet to maintain order in set
        Set<Character> s=new LinkedHashSet<>();
        for(char ch:str.toCharArray()){
            s.add(ch);
        }
        StringBuilder sb=new StringBuilder();
        for(char c:s){
            sb.append(c);
        }
        return String.valueOf(sb);
    }
}
