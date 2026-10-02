class Solution {
    public String convert(String s, int numRows) {
        if (numRows == 1 || s.length() <= numRows) {
            return s;
        }
        String[] c = new String[numRows];
        for (int i = 0; i < c.length; i++) {
            c[i] = "";
        }
        int cr = 0;
        boolean g = true;
        for (char ch : s.toCharArray()) {
            c[cr] += ch;
            if (cr == 0) {
                g = true;
            }
            if (cr == numRows - 1) {
                g = false;
            }
            cr += g ? 1 : -1;
        }
        String f = "";
        for (String a : c) {
            f += a;
        }
        return f;
    }
}
