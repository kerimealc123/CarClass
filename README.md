# CarClass

public class cars {

    //properties
    private Integer model;
    private String color;
    private String packet;
    private Integer maxSpeed;
    private Integer speed =0;
    private Integer brake =0;
    
    //setter method
    
    public void setModel(Integer model){
         this.model = model;
          }
    
    public void setColor(String color){
            this.color=color;
     
          }
    
    public void setPacket(String packet){
        this.packet=packet;
         }
    
    public void setMaxSpeed(INteger maxSpeed){
          this.maxSpeed=maxSpeed;
         }
    
    
    //getter method
   
    public Integer getModel(){
        return model;
    }
    
    public String getColor(){
        return color;
    }
    
    public String getPacket(){
        return packet;
    }
    
    public Integer getMaxSpeed(){
        return maxSpeed;
    }
    
    public void run(){
        System.debug('the car is running.');
    }
    public void stop(){
        System.debug('the car is stopped.');
    }
    public Integer acceleration(Integer accelerate){
        speed=accelerate+speed;
        if(speed<maxSpeed){
            System.debug('current speed'+speed);
        }else{
            System.debug('current speed'+maxSpeed);
        }
        return speed;
    }

    public INteger brake(Integer brake){
        speed= speed - brake;
        if(speed>0){
            System.debug('current speed'+speed);
        }else{
            System.debug('current speed:0 ');
        }
        
        return speed;
    }
}
