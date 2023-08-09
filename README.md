# question_one
 * @author abrar
 */
public class employee {
    String employeeType;
    String Name;
    String Position;
    double Salary;
    int Experience;
    String Educational_Level;
    public employee(String employeeType,String Name,String Position, double Salary,
    int Experience,String Educational_Level)
    {
    this.Salary = Salary+(Salary*0.5*Experience);
    switch(Educational_Level){
            case"Bachelor" -> this.Salary=this.Salary+500;
            case "diploma" -> this.Salary=this.Salary+250;
                        }
     switch(employeeType){
            case"Full time" -> this.Salary=this.Salary+(this.Salary*0.03);
            case "Part Time" -> this.Salary=this.Salary+(this.Salary*0.015);
                        }
  }
    
}

