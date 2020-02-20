# file

//For ==> index
val items = listOf(1, 22, 83, 4)  
   for ((index, value) in items.withIndex()) {
      println("the element at $index is $value")  //index la chi so p.tu
   }
   
   
   
//ForEach,  ForEachIndexed : arrayOf, listOf, mapOf
  for (i in items) println("values of the array"+i)
  listNumbers.forEach {it: Int // or  num ->
            if(it % 2 == 0){
                Log.d("AAAAA", it.toString())
            }
        }
  listNumbers.forEachIndexed { index, i ->
            Log.d("AAAAA", i.toString() + " index ->" + index)
        }
   listNumber.first()
   listNumber.last()
   ................
   
   
   
   
//Continue & Break phai sd labelName@ o dau vong lap
   myLabel@ for(x in 1..10) { // appling the custom label
      if(x = = 5) {
         println("I am inside if block with value"+x+"\n-- hence it will close the operation")
         break@myLabel //specifing the label
      } else {
         println("I am inside else block with value"+x)
         continue@myLabel
      }
   }
 
 
 //Interface 
 interface A
 var B: A = object:A{overrise}
 
 
 //------------------Function--------------------
 fun A: Unit { 
    //Unit don't turn anything == void
 }
 
fun A: String = "Huynh Thanh Duyen"

fun A: String? { 
    //cho phep return null
    return null
 }
 
//-------------Multible argument in function ==> ------------VARARG  -------------using *list-------- arrayOf NOT listOf--------
fun SayHello(chao:String, vararg arguments:String){
            arguments.forEach { arg ->
            //arguments luc nay la mot Array chua tat ca cac argment truyen vao
                Log.d("bbbbb", "$chao $arg")
            }
        }
var listMonhoc = arrayOf<String>("Toan", "Van", "Hoa hoc")
// SayHello("Chao", "Toan", "Van", "Hoa hoc")
// SayHello("Chao", *listMonhoc) 
   SayHello(chao = "Chao", arguments = *listMonhoc)  // tao tham so cu the thi truyen ca 2 
 
// -------------Get & set == gettter setter + xu ly in java --------------
var id:String? = "dsdsds"
        set(value) {
            field = value
            Log.d("AAAA", "ID id $value")
        }
        get() {
            Log.d("AAAA", "ID id $field")
            return field
        }

// ---------------------companion object---------------------
class a{
   companion object A {
      var a: String = "dfdfd"
      fun ActionMethod(){}
   }
}
==>  var b a.ActionMethod()  goi truc tiep khong can thong qua Object A
