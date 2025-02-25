# -Exercises-using-collection-framework---HashMap-and-Hashtable
import java.util.HashMap;
import java.util.Hashtable;
import java.util.Map;
import java.util.Scanner;
    public static void main(String[] args) {
               Map<String,Integer>hashMap=new HashMap<>();
        Map<String,Integer>hashtable=new Hashtable<>();
        Scanner scanner = new Scanner(System.in);
System.out.print("Enter key-value pairs (key1=value1 key2=value2 ...): ");
String input = scanner.nextLine();
String[] keyValuePairs = input.split("\\s+");
for (String pair : keyValuePairs) {
String[] keyValue = pair.split("=");
if (keyValue.length == 2) {
String key = keyValue[0];
int value = Integer.parseInt(keyValue[1]);
hashMap.put(key, value);
hashtable.put(key, value);
}
}
System.out.println("HashMap: " + hashMap);
System.out.println("Hashtable: " + hashtable);
scanner.close();
}
}
    
    

Output

Enter key-value pairs (key1=value1 key2=value2 ...): name= Anu city=coimbatore
HashMap: {name=Anu, city=coimbatore}
Hashtable: {name=Anu, city=coimbatore}

