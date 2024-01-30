# learning-about-object-methods

#Let's go back to Mark and John comparing their BMIs!  This time, let's use objects to implement the calculations! Remember: BMI = mass / (height * height) (mass in kg and #height in meters).  Your tasks:      For each of them, create an object with properties for their full name, mass, and height (Mark Miller and John Smith). Name these objects #as mark and john, and their properties exactly as fullName, mass and height.      Create a calcBMI method on each object to calculate the BMI (the same method on both #objects). Assign the BMI value to a property, and also return it from the method.      Log to the console who has the higher BMI, together with the full name and the #respective BMI. Example: "John Smith's BMI (28.3) is higher than Mark Miller's (23.9)!".  TEST DATA: Marks weighs 78 kg and is 1.69 m tall. John weighs 92 kg and is 1.95 m #tall.



const mark = {
    fullname : 'mark millar',
    mass : 78,
    height : 1.69,
    calBmi : function() {
        this.bmi = this.mass / this.height**2;
        return this.bmi
    }
    
    
};
const john = {
    fullname : 'john smiths',
    mass : 92,
    height : 1.95,
    calBmi : function() {
        this.bmi = this.mass / this.height**2;
        return this.bmi
    }

};


mark.calBmi();
john.calBmi();
console.log(mark.bmi, john.bmi);

// John Smith's BMI (28.3) is higher than Mark Miller's (23.9)!".

if (mark.bmi > john.bmi){
    console.log(`${mark.fullname} is BMI (${mark.bmi}) is higher than ${john.fullname} BMI (${john.bmi})`)
}else{
    
    console.log(`${john.fullname} is BMI (${john.bmi}) is higher than ${mark.fullname} BMI (${mark.bmi})`)

}

