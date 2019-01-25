package Project;
import javafx.application.Application;
import javafx.geometry.Insets;
import javafx.scene.Scene;
import javafx.scene.control.Button;
import javafx.scene.control.Label;
import javafx.scene.control.TextField;
import javafx.scene.layout.GridPane;
import javafx.stage.Stage;

public class MetricConverter extends Application{
    Stage window;
    Scene scene1, scene2;

    public static void main(String[] args){
        launch(args);
    }

    @Override
    public void start(Stage primaryStage) throws Exception {

         window = primaryStage;

        TextField input = new TextField();
        Button button1 = new Button("Convert");
        Button button2 = new Button("Convert");
        Button button3 = new Button("Convert");
        Button button4 = new Button("Convert");
        Button button5 = new Button("Convert");
        Button button6 = new Button("Convert");
        Button button7 = new Button("Convert");
        Button button8 = new Button("Convert");

        GridPane grid = new GridPane();
        grid.setPadding(new Insets(10,10,10,10));
        grid.setVgap(8);
        grid.setHgap(10);
        Label titleLabel = new Label("Convert: ");
        Label option1 = new Label("1. Km to Miles");
        Label option2 = new Label("2. Miles to Km");
        Label option3 = new Label("3. Celsius to Fahrenheit");
        Label option4 = new Label("4. Fahrenheit to Celsius");
        Label option5 = new Label("5. Kg to pounds");
        Label option6 = new Label("6. pounds to Kg");
        Label option7 = new Label("7. Meters to Feet");
        Label option8 = new Label("8. Feet to Meters");


        GridPane.setConstraints(titleLabel,0,0);
        GridPane.setConstraints(option1,0,1);
        GridPane.setConstraints(button1,1,1);

        GridPane.setConstraints(option2,0,2);
        GridPane.setConstraints(button2,1,2);

        GridPane.setConstraints(option3,0,3);
        GridPane.setConstraints(button3,1,3);

        GridPane.setConstraints(option4,0,4);
        GridPane.setConstraints(button4,1,4);

        GridPane.setConstraints(option5,0,5);
        GridPane.setConstraints(button5,1,5);

        GridPane.setConstraints(option6,0,6);
        GridPane.setConstraints(button6,1,6);

        GridPane.setConstraints(option7,0,7);
        GridPane.setConstraints(button7,1,7);

        GridPane.setConstraints(option8,0,8);
        GridPane.setConstraints(button8,1,8);

        TextField initialValue = new TextField();
        initialValue.setPromptText("Initial value");
        GridPane.setConstraints(initialValue,1, 0);
        button1.setOnAction(e -> AlertBox.display("Result",kmToMile(Double.parseDouble(initialValue.getText()))));
        button2.setOnAction(e -> AlertBox.display("Result",milteToKm(Double.parseDouble(initialValue.getText()))));
        button3.setOnAction(e -> AlertBox.display("Result",celsiusToF(Double.parseDouble(initialValue.getText()))));
        button4.setOnAction(e -> AlertBox.display("Result",fToCelsius(Double.parseDouble(initialValue.getText()))));
        button5.setOnAction(e -> AlertBox.display("Result",kgToLb(Double.parseDouble(initialValue.getText()))));
        button6.setOnAction(e -> AlertBox.display("Result",lbToKg(Double.parseDouble(initialValue.getText()))));
        button7.setOnAction(e -> AlertBox.display("Result",mToFt(Double.parseDouble(initialValue.getText()))));
        button8.setOnAction(e -> AlertBox.display("Result",ftToM(Double.parseDouble(initialValue.getText()))));


        grid.getChildren().addAll(titleLabel,option1,option2,option3,option4,option5,option6,option7,
                option8,button1,button2,button3,button4,button5,button6,button7,button8,initialValue);

        Scene scene = new Scene(grid,300,200);
        window.setScene(scene);
        window.setTitle("Metric Converter");
        window.show();

    }




    public String kmToMile(double input){
        return input + " Km = "+input * 0.62137 +" Miles";

    }
    public String milteToKm(double input){
        return input + " Miles = " + input/0.62137 +" Km";
    }
    public String celsiusToF(double input){
        return input + " Celsius = " + (input*1.8000 + 32.00) +" Fahrenheit";
    }
    public String fToCelsius(double input){
        return input + " Fahrenheit = " +(input-32.00)/1.8000+ " Celsius";
    }
    public String kgToLb(double input){
        return input+ " kg = "+input*2.2046+" pounds";
    }
    public String lbToKg(double input){
        return input + " pounds = "+input/2.2046+" kg";
    }
    public String mToFt(double input){
        return input+ " Meters = "+ input*3.2808+" Feet";
    }
    public String ftToM(double input){
        return (input + " ft = " + input/3.2808)+" Meters";
    }


}
