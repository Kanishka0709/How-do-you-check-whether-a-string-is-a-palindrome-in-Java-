# How-do-you-check-whether-a-string-is-a-palindrome-in-Java-
import java.util.*;
public class Main {
  public static void main(String[] args) {

    String str = "oppo";
    String reverseStr = "";

    int strLength = str.length();

    for (int i = (strLength - 1); i >=0; i--) 
    {
      reverseStr = reverseStr + str.charAt(i);
    }

    if (str.toLowerCase().equals(reverseStr.toLowerCase())) {
      System.out.println(str + "= Palindrome String");
    }
    else {
      System.out.println(str + "= not a Palindrome String");
    }
  }
}
