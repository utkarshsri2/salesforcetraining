<aura:application >

        
       
    <aura:attribute name ="wholenumber" type="Integer" access="public"/>
    <aura:attribute name ="percentage" type="Integer" access="public"/>
    
    <div> 
        <lightning:input type="number" name="input1" label="Enter a Whole number" 
                         value="{!v.wholenumber}"/>
        <lightning:input type="number" name="input12" label="Enter a percentage" 
                         value="{!v.percentage}" formatter="percent-fixed"  />
        
        
        {!div(mult(v.wholenumber,v.percentage),100)}
        
         
  
    
    </div>