# TipDonusumleri

'''namespace tipdonusumleri


{

class Program


    {
        static void Main(string[] args)
        {
        
//Implicit Conversion (Bilincsiz Dönüsüm)//


       byte a = 5;
       sbyte b =30;
       short c =10;

       int d =a+b+c;
       Console.WriteLine("d:"+d);

       long h =d;
       Console.WriteLine("h:" +h);

       float i =h;
       Console.WriteLine("i:" +i);

       string e= "ayse";
       char f = 'k';
       object g = e+f+d;
      Console.WriteLine("g:" +g);

//Explicit Conversion(Bilincli Dönüsüm)//

int x = 4;
byte y = (byte)x;
 Console.WriteLine("y:" +y);

 int z = 100;
 byte t = (byte)z;
 Console.WriteLine("t:" +t);

 float w = 10.3f;
 byte v = (byte)w;
  Console.WriteLine("v:" +v);

// *** ToString Methodu aldigi veriye stringe test eder.//


 //***** ToString Methodu*******")//

 int xx = 6;
 
 string yy =xx.ToString();
 
Console.WriteLine("yy:" +yy);

string zz = 12.5f.ToString();

Console.WriteLine("zz:" +z);


 //****System.Convert Methodu*****//
 
 
 //"******System.Convert Methodu***********")//

 string s1 = "10", s2 = "20"; //Ayni anda iki String  tanimlama!!!!!! Bu sekilde tek satirda birden fazla veri tanimlamsi yapilabilir.***//
 int sayi1, sayi2;
 int Toplam;

 sayi1 = Convert.ToInt32(s1);
 sayi2 = Convert.ToInt32(s2);

 Toplam = sayi1 + sayi2 ;
 Console.WriteLine("Toplam:" +Toplam);

// ********Parse methodu kullanmak******//
  
  ParseMethod();

  } 
 
 // Degisken isimleri tükendi ve dahafazla yaratici olamiycaz.Burda dikkat eddilmesi gereken önemli mevzu ayin degisken isimlerini ayni kod blogu üzerinde birden fazla kez kullanilmiyacagi bu durumda farkli bir kod blogu acip ayni degiskenleri kullanmaya devam edebiliriz.burda ayri bir fonsiyon oluyturuyoruz, cünkü main icinden cagirmazsam hicbir kod blogu calismiycak.//

  public static void ParseMethod()
  
  {
    string metin1 ="10";
    string metin2 = "10,25";
    int rakam1;
    double double1;
    
    rakam1 = Int32.Parse(metin1); //Burda string bir degiskeni pars kullanarak integer bir ifadeye dönüstürdük.
    double1 = Double.Parse(metin2);// string ifadenin double ifadeye dönüstürülmesi.


    Console.WriteLine("rakam1:" +rakam1);
    Console.WriteLine("double1:" +double1);

}}}'''
