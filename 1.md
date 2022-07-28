### Question
Given a list of numbers and a number k, return whether any two numbers from the list add up to k.

For example, given [10, 15, 3, 7] and k of 17, return true since 10 + 7 is 17.

### Solution

```java
package ListAddition;

/**
 * ListAddition
 */

public class ListAddition {

    public static boolean listAdd(int k, int[] list) {
        for (int i = 0; i < list.length; i++) {
            for (int j = i + 1; j < list.length; j++) {
                if (list[i] + list[j] == k) {
                    return true;
                }
            }
        }
        return false;
    }

    public static void main(String[] args) {
        int[] list = { 10, 15, 3, 7 };

        System.out.println(listAdd(17, list));
    }
}

```