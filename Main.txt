import java.util.ArrayList;

public class Main {
    public static int linearSearch(ArrayList<Integer> myarraylist, int value) {
        for (int i = 0; i < myarraylist.size(); i++) {
            if (myarraylist.get(i) == value) {
                return i;
            }
        }
        return -1;
    }

    public static void main(String[] args) {
        ArrayList<Integer> myarraylist = new ArrayList<Integer>();
        int[] arraycontents = { 5, 2, 8, 3, 6, 7, 1, 9, 4 };
        int i;
        for (i = 0; i < arraycontents.length; i++) {
            myarraylist.add(arraycontents[i]);
        }
        System.out.print(linearSearch(myarraylist, 6) + ", " + linearSearch(myarraylist, 5) + ", "
                + linearSearch(myarraylist, 4) + ", " + linearSearch(myarraylist, 100));
    }
    /*
     * 4) d
     * 5) a
     */
}