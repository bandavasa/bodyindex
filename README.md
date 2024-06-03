# MAIN 
public class Main {
    public static void main(String[] args) {
        BmiService service = new BmiService();
        int weight = 80;
        int height = 170;
        double d = (double) height / 100;


        double bmi = service.calculate(weight, d);
        System.out.println(bmi);
    }
}

# BmiService
public class BmiService {
    public double calculate(int kg, double m) {
        double result = kg / (m * m);


        return result;
    }
}