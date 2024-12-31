import java.io.File; import java.util.Scanner; public class Roll_27_8{ public static void
main(String[] args) { int sum = 0; File f = new File("C:\\Users\\sairaj\\Desktop\\sairaj.txt"); try{
Scanner fileScanner = new Scanner(f); while (fileScanner.hasNextLine()) { String line =
fileScanner.nextLine().trim(); // Read each line and trim any extra spaces try { int num =
Integer.parseInt(line); sum += num; } catch (Exception e) { System.out.println("Invalid Data in
file!!"+e); } } System.out.println("Total sum : " + sum); } catch (Exception e) {
System.out.println("Something Went Wrong!! check your file path..."); } } } /*OUTPUT * Total sum
: 100 */
