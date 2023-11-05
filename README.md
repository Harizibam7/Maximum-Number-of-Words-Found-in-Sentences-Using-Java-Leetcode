# Maximum-Number-of-Words-Found-in-Sentences-Using-Java-Leetcode
    class Solution {
        public int mostWordsFound(String[] sentences) {
            int max_length=0;
            for(String letter: sentences){
                int current_length = letter.split(" ").length;
                if(current_length>max_length){
                    max_length = current_length;
                }
            }
            return max_length;
        }
    }
