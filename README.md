import java.io.*;

class Student {

    String cname;
    int roll;
    String uname;
    String ename;

    InputStreamReader in = new InputStreamReader(System.in);
    BufferedReader br = new BufferedReader(in);

    void input() throws IOException {
        System.out.print("Enter Student Name:");
        cname= br.readLine();

        System.out.print("Enter Roll Number:");
        roll = Integer.parseInt(br.readLine());

        System.out.print("Enter Age:");
        uname = br.readLine();
       
        System.out.print("Enter Vaccine status:");
        ename = br.readLine();
    }
}

class Main extends Student {

    void display() {
        System.out.print("\nName..." + cname);
        System.out.print("\nRoll Number is.." + roll);
        System.out.print("\nAge is.." + uname);
        System.out.print("\nVaccine status is.." + ename);
       
    }

    public static void main(String args[]) throws IOException {
        Main c = new Main();
        c.input();
        c.display();
    }
}

