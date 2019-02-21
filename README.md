# palindrome

using System;

public class Palindrome
{
    public static bool IsPalindrome(string word)
    {
        try{
            char[] charArray = word.ToLower().ToCharArray();
            Array.Reverse(charArray);            
            return new string(charArray) == word.ToLower();            
        } catch{
            throw new NotImplementedException("Waiting to be implemented.");
        }
    }

    public static void Main(string[] args)
    {        
        Console.WriteLine(Palindrome.IsPalindrome("Deleveled"));
    }
}
