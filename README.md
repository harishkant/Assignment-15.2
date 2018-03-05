# Assignment-15.2


3.Write a partial function to add three numbers in which one number is constant and two
numbers can be passed as inputs and define another method which can take the partial
function as input and squares the result.

object MainObject {  
   def main(args: Array[String]) = {  
     functionExample(25, multiplyBy2)                   // Passing a function as parameter  
    }  
    def functionExample(a:Int, f:Int=>AnyVal):Unit = {  
        println(f(a))                                   // Calling that function   
    }  
    def multiplyBy2(a:Int):Int = {  
        a*2  
    }  
}


Output:

60


4.Write a program to print the prices of 4 courses of Acadgild: Android-12999,Big Data
Development-17999,Big Data Development-17999,Spark-19999 using match and add a
default condition if the user enters any other course.


object MainObject{  
    def main(args:Array[String]){  
        var map = Map(("Android",12999),("big data Development",17999),("spark",19999))  
        var map2 = Map("Andriod"->"12999","big data Development"->"17999","spark"->"19999")  
        var emptyMap:Map[String,String] = Map.empty[String,String]   
        println(map)  
        println(map2)  
        println("Empty Map: "+emptyMap)  
    }  
} 
