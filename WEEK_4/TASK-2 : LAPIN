import java.util.*;

class Codechef {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int T = sc.nextInt();

        while (T-- > 0) {
            String s = sc.next();
            int n = s.length();
            int mid = n / 2;

            String left = s.substring(0, mid);
            String right;

            if (n % 2 == 0) {
                right = s.substring(mid);
            } else {
                right = s.substring(mid + 1);
            }

            if (isLapindrome(left, right)) {
                System.out.println("YES");
            } else {
                System.out.println("NO");
            }
        }
        sc.close();
    }

    static boolean isLapindrome(String a, String b) {
        int[] freq = new int[26];

        for (char c : a.toCharArray()) {
            freq[c - 'a']++;
        }
        for (char c : b.toCharArray()) {
            freq[c - 'a']--;
        }

        for (int f : freq) {
            if (f != 0) return false;
        }
        return true;
    }
}
