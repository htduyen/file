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




//-----------------------------thua ke -----------------------------
constructor(name: String, old: Int, grade:Int):super(name,old){
        this.grade = grade
    }

// Serilizable đối tượng khi putIntent ==> getSerilizable()

//SharePreference 
var sharePrefence = getSharePrefenc("name_pref", Context.MODE_PRIVATE)
var edior = sharePrefencr.editor()
editor.putString("name", "Huynh Thanh Duyen")

==> Get SharePrefernce
var sharePrefence = getSharePrefenc("name_pref", Context.MODE_PRIVATE)
var getName = shareReerence.getString("name")


//https://github.com/winneze1/myapi2
Load image: Glide > picasso > Coil : About speed  

//Retrofit
    implementation 'androidx.recyclerview:recyclerview:1.2.0-alpha01'
    implementation 'androidx.cardview:cardview:1.0.0'

    implementation 'com.squareup.retrofit2:retrofit:2.7.1'
    implementation 'com.squareup.retrofit2:converter-gson:2.7.1'
    implementation 'com.squareup.retrofit2:adapter-rxjava2:2.7.1'

    implementation 'com.google.code.gson:gson:2.8.6'
    implementation 'com.github.bumptech.glide:glide:4.11.0'

    implementation 'androidx.lifecycle:lifecycle-extensions:2.2.0'
    implementation 'androidx.paging:paging-runtime:2.1.1'
    //Rx
    implementation 'io.reactivex.rxjava2:rxjava:2.2.7'
    implementation 'io.reactivex.rxjava2:rxandroid:2.1.1'

// holder.txtContent.text = StringBuilder(listPost[position].body.subSequence(0,20)).append("...").toString()

UI Github
Toast                      ==>   https://github.com/code-mc/loadtoast
SearchView                 ==>   http://miguelcatalan.info/2015/09/23/MaterialSearchView/
AnimationView              ==>   https://github.com/daimajia/AndroidViewAnimations
ImageSlide                 ==>   https://github.com/daimajia/AndroidImageSlider
CircleIndicator(Slide)     ==>   https://github.com/ongakuer/CircleIndicator
Material animation(activity   ==>   https://github.com/lgvalle/Material-Animations
Youtube: https://www.youtube.com/watch?v=RCLNkSIQQaw (ROOM CRUD + LiveData)

