package com.company;

import java.util.Arrays;
import java.util.Scanner;

public class Main {
    static Scanner input = new Scanner(System.in);

    public static void main(String[] args) {
        System.out.print("Введите строку ");
        String[] str = code(input.nextLine());
        for (String i : str
        ) {
            System.out.print(i);
        }
        System.out.println("\n" + decode(str));

    }

    public static String[] code(String string) {
        char[] newString = string.toCharArray();
        String[] codedString = new String[newString.length];

        for (int i = 0; i < codedString.length; i++) codedString[i] = Integer.toBinaryString(newString[i] - '0');
        reverseValueInStringArr(codedString);
        return codedString;
    }

        public static String decode(String[] code){
        reverseValueInStringArr(code);
        String string = "";
        for (String i :code
        ) {
            string += (char) + (fromBinToInt(i.toCharArray() ) + '0');
        }
        return string.replace('/',' ');
    }
    public static void reverseValueInStringArr(String[] arr){
        for(int i = 0; i < arr.length; i++){
            arr[i] = new StringBuilder(arr[i]).reverse().toString();
        }
    }
    public static int fromBinToInt(char[] arg) {

        int numb = 0;
        for (int i = 0; i < arg.length; i++) {
            numb += (arg[i] - '0') * (Math.pow(2, arg.length - 1 - i));
        }
        return numb;
    }
}


