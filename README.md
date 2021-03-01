# Library-Management-System-Code
To update the record of existing and issued library books by entering student ID number. The system issued the book by keeping the student’s current and previous records, simultaneously updating the database. 
-------CODE------
#include<iostream>
#include<fstream>
using namespace std;
class Database_Library
{
	protected :
	string common[30]={"oop", "ena", "english", "islamiyat","urdu","chemistry","lca","physics","dld" ,"edc" ,"signal","co","algebra","workshop","calculus","bme","cad","thermo","math","arabic" ,"statics","quran_majeed","allama_iqbal","dewan_e_ghalib","optics","laser","therapy","anatomy","seeret_e_nabi","it"};
	string software_section[10]={"software_books","aalgorithem","clean_code","craftsmanship","ageli","clean_coder","coder","decoder","pro_git","beautiful_code"};
	string manager[10]={"terrorism" ,"islam" , "science" ,"socilism","psychology", "political","ww1", "tourism","bride_of_pak","jinnah"};	 		
	string d1[10]={"pakistan_history","m_ali_jinnah","prgramming","looping","nested","algorithem","hacking","nested_loop","if_else","logic",};
	string d2[10]={"eletrical_engineering","network_analysis","superposition","super_node","kcl","kvl","nodes","electric_networking","magnatization","electricity"};
	string d3[10]={"sperms","ecosyststem","dead_bodies","food_chain","biotic","nonbiotic","food_web","seeds","redical","reproduction"};
	string d4[10]={"news","web","newscaster","journalist","nest","journalism","organizational","breaking_news","mid_news","shows"};
	string d5[10]={"aero","engines","planes","helicopter","ships","air","uniform","air_performance","control_t","tower"};   
    public :
	void ss(){
	cout<<"                                         ***                                                                                              ***"<<endl;
	cout<<"                                                     -:      SOFTWARE  SECTION  HAS  BOOKS  ONLY  THESE BOOKS  IN  SOFT FORM     :-       "<<endl;
	cout<<"                                         ***                                                                                              ***"<<endl;
	for (int i=0;i<10;i++)
	cout<<"   Book number "<<i+1<<"    "<<software_section[i]<<endl;
	cout<<endl;
	cout<<"This book"<<"  "<<software_section[6]<<" "<<" has concerned software  with  [ D-CompileR ] "<<endl; 
	cout<<"This book"<<"  "<<software_section[5]<<" "<<" has concerned software  with    [ Dev-C++ ] "<<endl; 
	cout<<endl;
	cout<<"Soory! Remaining books have no  more concerned  softwares  "<<endl;}
	void Library_books2(){
	cout<<"                                                        W  E  L  C  O  M  E          T  O         L I  B  R  A  R Y                         "<<endl;
	for (int i=0;i<30;i++)
	cout<<"   Book number "<<i+1<<"    "<<common[i]<<endl;
	cout<<endl;
	cout<<endl;
	cout<<"                                       ***                                                               ***"<<endl;
	cout<<"                                                     -:      MANAGER HAS ONLY THESE BOOKS     :-       "<<endl;
	cout<<"                                       ***                                                               ***"<<endl;
	for (int i=0;i<10;i++)
	cout<<"   Book number "<<i+1<<"    "<<manager[i]<<endl;
	cout<<endl;}
	void Library_books(){
	ofstream file2;
	file2.open("d:\\Library_Books.txt", ios::trunc);
	if (file2.is_open())
	{
	file2<<"                                                        W  E  L  C  O  M  E          T  O         L I  B  R  A  R Y                         "<<endl;
	for (int i=0;i<30;i++)
	file2<<"   Book number "<<i+1<<"    "<<common[i]<<endl;
	file2.close();}
	else cout<<"error";
    }
    void Library_books123(){
	ofstream file;
	file.open("d:\\Manager_Books.txt", ios::trunc);
	if (file.is_open())
	{

	file<<"                                       ***                                                               ***"<<endl;
	file<<"                                                     -:      MANAGER HAS ONLY THESE BOOKS     :-       "<<endl;
	file<<"                                       ***                                                               ***"<<endl;
	for (int i=0;i<10;i++)
	file<<"   Book number "<<i+1<<"    "<<manager[i]<<endl;
	file<<endl;
	file.close();}
	else 
	cout<<"error";
    }
	void computer_sc(){
	cout<<"                                       ***                                                                           ***"<<endl;
	cout<<"                                                   -:      COMPUTER SCIENCE DEPARTMENT HAS  THESE BOOKS     :-       "<<endl;
	cout<<"                                       ***                                                                           ***"<<endl;
	for (int i=0;i<10;i++)
	cout<<"   Book number "<<i+1<<"    "<<d1[i]<<endl;
	cout<<endl;
	cout<<endl;}
    void electrical_eng(){
	cout<<"                                       ***                                                                           ***"<<endl;
	cout<<"                                                   -:      ELETRICAL ENGINEERING DEPARTMENT HAS THESE BOOKS     :-       "<<endl;
	cout<<"                                       ***                                                                           ***"<<endl;
	for (int i=0;i<10;i++)
	cout<<"   Book number "<<i+1<<"    "<<d2[i]<<endl;
	cout<<endl;}
    void medical(){
	cout<<"                                       ***                                                                           ***"<<endl;
	cout<<"                                                   -:      MEDICAL DEPARTMENT HAS THESE BOOKS     :-       "<<endl;
	cout<<"                                       ***                                                                           ***"<<endl;
	for (int i=0;i<10;i++)
	cout<<"   Book number "<<i+1<<"    "<<d3[i]<<endl;
	cout<<endl;
	cout<<endl;}	
    void aviation_man(){
	cout<<"                                       ***                                                                           ***"<<endl;
	cout<<"                                                     -:      AVIATION DEPARTMENT HAS THESE BOOKS     :-       "<<endl;
	cout<<"                                       ***                                                                           ***"<<endl;
	for (int i=0;i<10;i++)
	cout<<"   Book number "<<i+1<<"    "<<d5[i]<<endl;
	cout<<endl;
	cout<<endl;}		
    void mass_com(){
	cout<<"                                       ***                                                                           ***"<<endl;
	cout<<"                                                   -:    MASS COMMUNICATION  DEPARTMENT HAS THESE BOOKS     :-           "<<endl;
	cout<<"                                       ***                                                                           ***"<<endl;
	for (int i=0;i<10;i++)
	cout<<"   Book number "<<i+1<<"    "<<d4[i]<<endl;
	cout<<endl;}
};
class software_section
{
public :
	    int date,month,year;
	    int ddate =0;
	    int idate=1;
		int b=-1;
		string z;
    string software_section[10]={"software_books","aalgorithem","clean_code","craftsmanship","ageli","clean_coder","coder","decoder","pro_git","beautiful_code"};	
    void ss()
	{
	ofstream file;
	file.open("d:\\software_Books.txt",ios ::trunc);
	if(file.is_open())
	{
	file<<"                                         ***                                                                                              ***"<<endl;
	file<<"                                                     -:      SOFTWARE  SECTION  HAS  BOOKS  ONLY  THESE BOOKS  IN  SOFT FORM     :-       "<<endl;
	file<<"                                         ***                                                                                              ***"<<endl;
	for (int i=0;i<10;i++)
	file<<"   Book number "<<i+1<<"    "<<software_section[i]<<endl;
	file<<endl;
	file<<"This book"<<"  "<<software_section[6]<<" "<<" has concerned software  with  [ D-CompileR ] "<<endl; 
	file<<"This book"<<"  "<<software_section[5]<<" "<<" has concerned software  with    [ Dev-C++ ] "<<endl; 
	file<<endl;
	file<<"Soory! Remaining books have no  more concerned  softwares  "<<endl;
	file.close();
}
else
cout<<"error";	
}
	void ss1(){
		cout<<"                                       ***                                                                           ***"<<endl;
		cout<<"                                                   -:      SOFTWARE  SECTION  DEPARTMENT  HAS  ONLY THESE BOOKS   IN  SOFT FORM     :-       "<<endl;
		cout<<"                                       ***                                                                           ***"<<endl;
		for (int i=0;i<10;i++)
		cout<<"   Book number "<<i+1<<"    "<<software_section[i]<<endl;
		cout<<endl;
		cout<<endl;
		cout<<"Enter book name you want to search :";
		cin>>z;
		cout<<endl;
		cout<<"You want this book in  Library :"<<z<<endl;
		for (int q=0;q<10;q++)
		if (software_section[q] ==z)
		b = q;
		if (b == -1){
			cout<<"Sorry! Your book is  not  found in Software  Library."<<endl;
			exit(-1);}
    	else
			{ 
				cout<<"Found in library "<<b+1<<"   "<<z<<endl;
				cout<<"Issue "<<b+1<<" number book  "<<z<<" to this student "<<endl;
      			cout<<"For issueing this book you must need to enter current date!"<<endl;
				cout<<"Enter Date :";
				cin>>date;
				cout<<"Enter month :";
				cin>>month;
				cout<<"Enter Year :";
				cin>>year;
				cout<<"                           ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"                           ****"<<endl;
		        cout<<endl;
				cout<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
				cout<<endl;
			    if (date<16)
	          	cout<<"                           ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"                       ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
		cout<<"                           ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"               ****"<<endl;
		}
        else
        {
	     ddate=(date+15) % 30;
	    cout<<"                           ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"                ****"<<endl;
		}
	    cout<<endl;
	    cout<<endl;
	    cout<<"                                                         You  have issue  this  book : "<<z<<endl;
		cout<<"                                       ***                                                                           ***"<<endl;
		cout<<"                                                   -:            UPDATED   SOFTWARE   LIBRARY      :-       "<<endl;
		cout<<"                                       ***                                                                           ***"<<endl;
		cout<<endl;
		cout<<endl;
		for (int q=0;q<10;q++){
	    	if (software_section[q] == z)
				{
					b = q;
					software_section[q][0]=NULL;
				}
		cout<<"Book number # "<<q+1<<"    "<<software_section[q]<<endl;
	}
	    		exit(-1);
	    }}		
};
class student :public Database_Library
{
	protected:
		int num=0;
		int z;
		int b=-1;
		string s,v;
		string std[30];
		public:
	    student()
	    {
	    std [0]  = "talha_33";
		std [1]  = "naveed_04";	
		std [2]  = "fakher_18";
		std [3]  = "ali_29";
		std [4]  = "sdaqat_34";
		std [5]  = "aqib_26";
		std [6]  = "hira_25";	
		std [7]  = "saad_6";
		std [8]  = "muzamil_23";
		std [9]  = "javed_39";	
		std [10] = "ihsan_30";	
		std [11] = "qaiser_40";
		std [12] = "khizer_14";
		std [13] = "maaz_47";
		std [14] = "remzan_37";	
		std [15] = "qasim_48";
		std [16] = "moeed_4";
		std [17] = "hamza_9";
		std [18] = "talal_15";	
		std [19] = "usman_51";
		std [20] = "haris_41";
		std [21] = "sajid_42";	
		std [22] = "zair_43";	
		std [23] = "khokher_31";
		std [24] = "umer_3";
		std [25] = "rafii_26";
		std [26] = "awais_45";	
		std [27] = "hafiz_talha_2";	
		std [28] = "mensoor_11";
		std [29] = "ahmad_10";
	}
    void input3()
	{
		cout<<"                                       ***                                                               ***"<<endl;
		cout<<"                                                     -:      L I B R A R I O N    :-       "<<endl;
		cout<<"                                       ***                                                               ***"<<endl;
		cout<<endl;
        cout<<"Enter  student   name   and  roll number :";
		cin>>s;
		cout<<"You are searching this student name in record  :"<<s<<endl;
		for (int q=0;q<30;q++)
		if (s==std[q]){
		b = q;}
		if (b == -1)
		{cout<<"Sorry! This student has not account in Library. Please go to account office and apply for library account!   " <<endl;
		exit(-1);}
    	else {
    	cout<<"Found in Record : "<<s<<endl;
    	cout<<endl<<endl;
		cout<<"If  your  Desire  to  see  books in  the  Departments  then  type  1;  otherwise you should go and issue Book! ";
		cin>>num;
		if(num ==1)
		{
		Database_Library ::computer_sc();	
		Database_Library ::electrical_eng();
		Database_Library ::medical();	
		Database_Library ::aviation_man();
		Database_Library ::mass_com();
		cout<<endl<<endl<<endl<<endl;	
		cout<<"                                                N O W      G O     A N D     I S S U E      B O O K  "<<endl;
		cout<<endl<<endl;}
		else
		cout<<"  "; }	
	}
};
class Department_1:public student
{
    public :
    string d1[20]={"hacking_c","loop","prgramming","looping","nested","algorithem","hacking","nested_loop","if_else","logic"};
   	string z1,w;
	int b=-1;
	int k,l;
	int date,month,year;
	int ddate =0;
	int idate=1;
	void computer_sc()
{
	ofstream file;
	file.open("d:\\CS_BookS.txt");
	if(file.is_open())
	{
		file<<"                                       ***                                                                           ***"<<endl;
		file<<"                                                   -:       COMPUTER SCIENCe  DEPARTMENT HAS THESE BOOKS     :-           "<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		for (int i=0;i<10;i++)
		file<<"   Book "<<d1[i]<<endl;
		file<<endl;
        file.close();	
}
else
cout<<"error";
}
    void computer_sc1()
    {
		cout<<endl;
		cout<<"Enter book name you want to search CS Library :";
		cin>>z1;
		cout<<endl;
		cout<<"You want this book in Library :"<<z1<<endl;
		for (int q=0;q<10;q++)
		if (d1[q] ==z1)
		b = q;
		if (b == -1){
		cout<<"Sorry! Your book is  not  found in    Library."<<endl;
		}
    	else
			{ 
				cout<<"Found in library "<<z1<<endl;
				cout<<"Issue  book  ("<<z1<<") to student!"<<endl;
      			cout<<"For issueing this book you must need to enter current date!"<<endl;
				cout<<"Enter Date :";
				cin>>date;
				cout<<"Enter month :";
				cin>>month;
				cout<<"Enter Year :";
				cin>>year;
		    	cout<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"                          ****"<<endl;
		        cout<<endl;
				cout<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
				cout<<endl;
			    if (date<16)
	    cout<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"                      ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else
        {
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;
		}
	    cout<<endl;
		fstream f;
		f.open("d:\\Fine.txt", ios::app);
		if(f.is_open())
		{
		f<<"Issue ("<<z1<<")to  this  student "<<std[b]<<endl; 
		f<<endl;
		f<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"              ****"<<endl;
		f<<endl;
		f<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
		f<<endl;
		if (date<16)
		f<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"              ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
		f<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else{
	    ddate=(date+15) % 30;
	    f<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;}
		f.close();	
		}
		else
		cout<<"error";
		cout<<endl;
        fstream file;
	    file.open("d:\\CS_BookS.txt", ios::trunc);
		file<<"                                                             You  have issue  this  book :    "<<z1<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		file<<"                                                          -:            UPDATED    COMPUTER SCIENCE   DEPARTMENT  LIBRARY      :-       "<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		file<<endl;
	    for (int q=0;q<10;q++){
	    if (d1[q] == z1)
			{b = q;
			d1[q]="This Book  is Issued";
			}
		file<<d1[q]<<endl;} 
		cout<<endl<<endl;
		cout<<"IF you want to add any new books in Library then type 'yes' !"<<endl;
		cin>>w;
		if(w  =="yes")
		{
		cout<<endl<<endl;
		cout<<"You can add  maximum 10 new books at a time!"<<endl;
		cout<<"How many books you want to enter? ";
		cin>>k;
			file<<"                                       ***                                                                           ***"<<endl;
	for (int j=10;j<10+k;j++)
	{
	
		cout<<"Enter new book :";
		cin>>d1[j];
		file<<d1[j]<<endl;
	}
	file.close();

}
	exit(-1);
	}
}   
};
class Department_2:public student{
    public :
    string d2[20]={"eletrical_engineering","network_analysis","superposition","super_node","kcl","kvl","nodes","electric_networking","magnatization","electricity"};
   	string z1,w;
	int b=-1;
	int k,l;
	int date,month,year;
	int ddate =0;
	int idate=1;
	void electrical_eng()
{
	ofstream file;
	file.open("d:\\EE_BookS.txt",ios ::trunc);
	if(file.is_open())
	{
		file<<"                                       ***                                                                           ***"<<endl;
		file<<"                                                   -:      ELETRICAL ENGINEERING  DEPARTMENT HAS THESE BOOKS     :-           "<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		for (int i=0;i<10;i++)
		file<<"   Book "<<d2[i]<<endl;
		file<<endl;
        file.close();	
}
else
cout<<"error";
}
    void electrical_eng1()
    {
		cout<<endl;
		cout<<"Enter book name you want to search   EE libray :";
		cin>>z1;
		cout<<endl;
		cout<<"You want this book in Library :"<<z1<<endl;
		for (int q=0;q<10;q++)
		if (d2[q] ==z1)
		b = q;
		if (b == -1){
		cout<<"Sorry! Your book is  not  found in    Library."<<endl;
		}
    	else
			{ 
				cout<<"Found in library "<<z1<<endl;
				cout<<"Issue  book  ("<<z1<<") to student!"<<endl;
      			cout<<"For issueing this book you must need to enter current date!"<<endl;
				cout<<"Enter Date :";
				cin>>date;
				cout<<"Enter month :";
				cin>>month;
				cout<<"Enter Year :";
				cin>>year;
		    	cout<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"                          ****"<<endl;
		        cout<<endl;
				cout<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
				cout<<endl;
			    if (date<16)
	    cout<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"                      ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else
        {
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;
		}
	    cout<<endl;
		fstream f;
		f.open("d:\\Fine.txt", ios::app);
		if(f.is_open())
		{
		f<<"Issue ("<<z1<<")to  this  student "<<std[b]<<endl; 
		f<<endl;
		f<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"              ****"<<endl;
		f<<endl;
		f<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
		f<<endl;
		if (date<16)
		f<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"              ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
		f<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else{
	    ddate=(date+15) % 30;
	    f<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;}
		f.close();	
		}
		else
		cout<<"error";
        fstream file;
	    file.open("d:\\EE_BookS.txt", ios::trunc);
		file<<"                                                             You  have issue  this  book :    "<<z1<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		file<<"                                                          -:            UPDATED   MEDICAL   DEPARTMENT  LIBRARY      :-       "<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		file<<endl;
	    for (int q=0;q<10;q++){
	    if (d2[q] == z1)
			{b = q;
			d2[q]="This Book  is Issued";
			}
		file<<d2[q]<<endl;} 
		cout<<endl<<endl;
		cout<<"IF you want to add any new books in Library then type 'yes' !"<<endl;
		cin>>w;
		if(w  =="yes")
		{
		cout<<endl<<endl;
		cout<<"You can add  maximum 10 new books at a time!"<<endl;
		cout<<"How many books you want to enter? ";
		cin>>k;
			file<<"                                       ***                                                                           ***"<<endl;
	for (int j=10;j<10+k;j++)
	{
	
		cout<<"Enter new book :";
		cin>>d2[j];
		file<<d2[j]<<endl;
	}
	file.close();

}
	exit(-1);
	}
}   
};
class Department_3:public student{
    public :
	string d3[20]={"sperms","ecosyststem","dead_bodies","food_chain","biotic","nonbiotic","food_web","seeds","redical","reproduction"};
   	string z1,w;
	int b=-1;
	int k,l;
	int date,month,year;
	int ddate =0;
	int idate=1;
	void medical()
{
	ofstream file;
	file.open("d:\\MEDICAL_BookS.txt",ios ::trunc);
	if(file.is_open())
	{
		file<<"                                       ***                                                                           ***"<<endl;
		file<<"                                                   -:      MEDICAL   DEPARTMENT HAS THESE BOOKS     :-           "<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		for (int i=0;i<10;i++)
		file<<"   Book "<<d3[i]<<endl;
		file<<endl;
        file.close();	
}
else
cout<<"error";
}
    void medical1()
    {
		cout<<"Enter book name you want to search  MEDICAL  Library :";
		cin>>z1;
		cout<<endl;
		cout<<"You want this book in Library :"<<z1<<endl;
		for (int q=0;q<10;q++)
		if (d3[q] ==z1)
		b = q;
		if (b == -1){
		cout<<"Sorry! Your book is  not  found in    Library."<<endl;
		}
    	else
			{ 
				cout<<"Found in library "<<z1<<endl;
				cout<<"Issue  book  ("<<z1<<") to student!"<<endl;
      			cout<<"For issueing this book you must need to enter current date!"<<endl;
				cout<<"Enter Date :";
				cin>>date;
				cout<<"Enter month :";
				cin>>month;
				cout<<"Enter Year :";
				cin>>year;
		    	cout<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"                          ****"<<endl;
		        cout<<endl;
				cout<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
				cout<<endl;
			    if (date<16)
	    cout<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"                      ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else
        {
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;
		}
	    cout<<endl;
		fstream f;
		f.open("d:\\Fine.txt", ios::app);
		if(f.is_open())
		{
		f<<"Issue ("<<z1<<")to  this  student "<<std[b]<<endl; 
		f<<endl;
		f<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"              ****"<<endl;
		f<<endl;
		f<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
		f<<endl;
		if (date<16)
		f<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"              ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
		f<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else{
	    ddate=(date+15) % 30;
	    f<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;}
		f.close();	
		}
		else
		cout<<"error";
		cout<<endl;
        	fstream file;
	    file.open("d:\\MEDICAL_BookS.txt", ios::trunc);
		file<<"                                                             You  have issue  this  book :    "<<z1<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		file<<"                                                          -:            UPDATED   MEDICAL   DEPARTMENT  LIBRARY      :-       "<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		file<<endl;
	    for (int q=0;q<10;q++){
	    if (d3[q] == z1)
			{b = q;
			d3[q]="This Book  is Issued";
			}
		file<<d3[q]<<endl;} 
		cout<<endl<<endl;
		cout<<"IF you want to add any new books in Library then type 'yes' !"<<endl;
		cin>>w;
		if(w  =="yes")
		{
		cout<<endl<<endl;
		cout<<"You can add  maximum 10 new books at a time!"<<endl;
		cout<<"How many books you want to enter? ";
		cin>>k;
			file<<"                                       ***                                                                           ***"<<endl;
	for (int j=10;j<10+k;j++)
	{
	
		cout<<"Enter new book :";
		cin>>d3[j];
		file<<d3[j]<<endl;
	}
	file.close();

}
	exit(-1);
	}
}   
};
class Department_4:public student{
    public :
    string d4[20]={"aero","engines","planes","helicopter","ships","air","uniform","air_performance","control_t","tower"}; 	
   	string z1,w;
	int b=-1;
	int k,l;
	string book1,book2,book3;
	int date,month,year;
	int ddate =0;
	int idate=1;
	void aviation_man()
{
	ofstream file;
	file.open("d:\\Aviation_BookS.txt",ios ::trunc);
	if(file.is_open())
	{
		file<<"                                       ***                                                                           ***"<<endl;
		file<<"                                                   -:      AVIATION   DEPARTMENT HAS THESE BOOKS     :-           "<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		for (int i=0;i<10;i++)
		file<<"   Book number "<<i+1<<"    "<<d4[i]<<endl;
		file<<endl;
        file.close();	
}
else
cout<<"error";
}
    void aviation_man1()
    {
		cout<<"Enter book name you want to search  AVIATION  library :";
		cin>>z1;
		cout<<endl;
		cout<<"You want this book in Library :"<<z1<<endl;
		for (int q=0;q<10;q++)
		if (d4[q] ==z1)
		b = q;
		if (b == -1){
		cout<<"Sorry! Your book is  not  found in  AVIATION   Library."<<endl;
		}
    	else
			{ 
				cout<<"Found in library "<<z1<<endl;
				cout<<"Issue  book  ("<<z1<<") to student!"<<endl;
      			cout<<"For issueing this book you must need to enter current date!"<<endl;
				cout<<"Enter Date :";
				cin>>date;
				cout<<"Enter month :";
				cin>>month;
				cout<<"Enter Year :";
				cin>>year;
		    	cout<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"                          ****"<<endl;
		        cout<<endl;
				cout<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
				cout<<endl;
			    if (date<16)
	    cout<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"                      ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else
        {
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;
		}
	    cout<<endl;
		fstream f;
		f.open("d:\\Fine.txt", ios::app);
		if(f.is_open())
		{
		f<<"Issue ("<<z1<<")to  this  student "<<std[b]<<endl; 
		f<<endl;
		f<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"              ****"<<endl;
		f<<endl;
		f<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
		f<<endl;
		if (date<16)
		f<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"              ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
		f<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else{
	    ddate=(date+15) % 30;
	    f<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;}
		f.close();	
		}
		else
		cout<<"error";
		cout<<endl;
        	fstream file;
	    file.open("d:\\Aviation_BookS.txt", ios::trunc);
		file<<"                                                             You  have issue  this  book :    "<<z1<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		file<<"                                                          -:            UPDATED   AVIATION   DEPARTMENT  LIBRARY      :-       "<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		file<<endl;
	    for (int q=0;q<10;q++){
	    if (d4[q] == z1)
			{b = q;
			d4[q]="This Book  is Issued";
			}
		file<<d4[q]<<endl;} 
		cout<<endl<<endl;
		cout<<"IF you want to add any new books in Library then type 'yes' !"<<endl;
		cin>>w;
		if(w  =="yes")
		{
		cout<<endl<<endl;
		cout<<"You can add  maximum 10 new books at a time!"<<endl;
		cout<<"How many books you want to enter? ";
		cin>>k;
			file<<"                                       ***                                                                           ***"<<endl;
	for (int j=10;j<10+k;j++)
	{
		cout<<"Enter new book :";
		cin>>d4[j];
		file<<d4[j]<<endl;
	}
	file.close();
}

	exit(-1);
	}
}   
};
class Department_5:public student{

     public :
   	string d5[20]={"news","web","newscaster","journalist","nest","journalism","organizational","breaking_news","mid_news","shows"};
   	string z1,w;
	int b=-1;
	int k,l;
	string book1,book2,book3;
	int date,month,year;
	int ddate =0;
	int idate=1;
	void mass_com()
{
	ofstream file;
	file.open("d:\\MASS_Communication_BookS.txt",ios ::trunc);
	if(file.is_open())
	{
		file<<"                                       ***                                                                           ***"<<endl;
		file<<"                                                   -:    MASS COMMUNICATION  DEPARTMENT HAS THESE BOOKS     :-           "<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		for (int i=0;i<10;i++)
		file<<"   Book number "<<i+1<<"    "<<d5[i]<<endl;
		file<<endl;
        file.close();	
}
else
cout<<"error";
}
    void mass_com1()
    {
		cout<<"Enter book name you want to search  MASS COMMUNICATION  Library :";
		cin>>z1;
		cout<<endl;
		cout<<"You want this book in Library :"<<z1<<endl;
		for (int q=0;q<10;q++)
		if (d5[q] ==z1)
		b = q;
		if (b == -1){
		cout<<"Sorry! Your book is  not  found in MASS COMMUNICATION  Library."<<endl;
		}
    	else
			{ 
				cout<<"Found in library "<<z1<<endl;
				cout<<"Issue  book  ("<<z1<<") to student!"<<endl;
      			cout<<"For issueing this book you must need to enter current date!"<<endl;
				cout<<"Enter Date :";
				cin>>date;
				cout<<"Enter month :";
				cin>>month;
				cout<<"Enter Year :";
				cin>>year;
		    	cout<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"                          ****"<<endl;
		        cout<<endl;
				cout<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
				cout<<endl;
			    if (date<16)
	    cout<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"                      ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else
        {
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;
		}
	    cout<<endl;
		fstream f;
		f.open("d:\\Fine.txt", ios::app);
		{
		f<<"Issue ("<<z1<<")to  this  student "<<std[b]<<endl; 
		f<<endl;
		f<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"              ****"<<endl;
		f<<endl;
		f<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
		f<<endl;
		if (date<16)
		f<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"              ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
		f<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else{
	    ddate=(date+15) % 30;
	    f<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;}
		f.close();	
		}
		cout<<endl;
		fstream file;
	    file.open("d:\\MASS_Communication_BookS.txt", ios::trunc);
		file<<"                                                             You  have issue  this  book :    "<<z1<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		file<<"                                                          -:            UPDATED  MASS COMMUNICATION  LIBRARY      :-       "<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		file<<endl;
	    for (int q=0;q<10;q++){
	    if (d5[q] == z1)
			{b = q;
			d5[q]="This Book  is Issued";
			}
		file<<d5[q]<<endl;} 
		cout<<endl<<endl;
		cout<<"IF you want to add any new books in Library then type 'yes' !"<<endl;
		cin>>w;
		if(w  =="yes")
		{
		cout<<endl<<endl;
		cout<<"You can add  maximum 10 new books at a time!"<<endl;
		cout<<"How many books you want to enter? ";
		cin>>k;
			file<<"                                       ***                                                                           ***"<<endl;
	for (int j=10;j<10+k;j++)
	{
		cout<<"Enter new book :";
		cin>>d5[j];
		file<<d5[j]<<endl;
	}
	file.close();
}

	exit(-1);
	}
}   
};
class manager : public student,public Database_Library
{
   public :
   	string manager[20]={"terrorism" ,"islam" , "science" ,"socilism","psychology", "political","ww1", "tourism","bride_of_pak","jinnah"};
   	string z1,w;
	int b=-1;
	int k,l;
	string book1,book2,book3;
	int date,month,year;
	int ddate =0;
	int idate=1;
    void manager1()
    {
		cout<<"Enter book name you want to search in Manager's Library :";
		cin>>z1;
		cout<<endl;
		cout<<"You want this book in Manager Library :"<<z<<endl;
		for (int q=0;q<10;q++)
		if (manager[q] ==z1)
		b = q;
		if (b == -1){
		cout<<"Sorry! Your book is  not  found in Manager's Library."<<endl;
		cout<<"Manager : Refer to  DepartmenT "<<endl;}
    	else
			{ 
				cout<<"Found in library "<<z1<<endl;
				cout<<"Issue  book  ("<<z1<<") to student!"<<endl;
      			cout<<"For issueing this book you must need to enter current date!"<<endl;
				cout<<"Enter Date :";
				cin>>date;
				cout<<"Enter month :";
				cin>>month;
				cout<<"Enter Year :";
				cin>>year;
		    	cout<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"                          ****"<<endl;
		        cout<<endl;
				cout<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
				cout<<endl;
			    if (date<16)
	    cout<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"                      ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else
        {
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;
		}
	    cout<<endl;
		fstream f;
		f.open("d:\\Fine.txt", ios::app);
		{
		f<<"Issue ("<<z1<<")to  this  student "<<std[b]<<endl; 
		f<<endl;
		f<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"              ****"<<endl;
		f<<endl;
		f<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
		f<<endl;
		if (date<16)
		f<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"              ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
		f<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else{
	    ddate=(date+15) % 30;
	    f<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;}
		f.close();	
		}
		cout<<endl;
		fstream file;
	    file.open("d:\\Manager_Books.txt", ios::trunc);
		file<<"                                                             You  have issue  this  book :    "<<z1<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		file<<"                                                          -:            UPDATED  MANAGER'S  LIBRARY      :-       "<<endl;
		file<<"                                       ***                                                                           ***"<<endl;
		file<<endl;
	    for (int q=0;q<10;q++){
	    if (manager[q] == z1)
			{b = q;
			manager[q]="This Book  is Issued";
			}
		file<<manager[q]<<endl;} 
		cout<<endl<<endl;
		cout<<"IF you want to add any new books in Library then type 'yes' !"<<endl;
		cin>>w;
		if(w  =="yes")
		{
		cout<<endl<<endl;
		cout<<"You can add  maximum 10 new books at a time!"<<endl;
		cout<<"How many books you want to enter? ";
		cin>>k;
			file<<"                                       ***                                                                           ***"<<endl;
	for (int j=10;j<10+k;j++)
	{
		cout<<"Enter new book :";
		cin>>manager[j];
		file<<manager[j]<<endl;
	}
	file.close();
}

	exit(-1);
	}
}   
};
class librarian :public student,public Database_Library
{
	public :
	string common[40]={"oop", "ena", "english", "islamiyat","urdu","chemistry","lca","physics","dld" ,"edc" ,"signal","co","algebra","workshop","calculus","bme","cad","thermo","math","arabic" ,"statics","quran_majeed","allama_iqbal","dewan_e_ghalib","optics","laser","therapy","anatomy","seeret_e_nabi","it"};
	int b=-1;
	int date,month,year;
	int ddate =0;
	int idate=1;
	int k,l;
	string b1,book1,book2,book3,w;
		void input3()
		{
		cout<<"Enter book you want to search in Library : ";
		cin>>b1;
		cout<<endl;
		cout<<"You want this book :"<<b1<<endl;
		for (int q=0;q<30;q++)
		if (common[q] == b1)
		b = q;
		if (b == -1)
		{
		cout<<"Sorry! Your book is  not  found in Library.You should go to manager perhapes your book is previliage type!"<<endl;
    	}
		else
		{ 
		cout<<"Found in library  "<<b1<<endl;
		cout<<"For issueing this book you must need to enter current date!   "<<endl;
		cout<<"Enter Date :";
		cin>>date;
		cout<<"Enter month :";
		cin>>month;
		cout<<"Enter Year :";
		cin>>year;
		cout<<endl;
		cout<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"              ****"<<endl;
		cout<<endl;
		cout<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
		cout<<endl;
		if (date<16)
		cout<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"              ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
		cout<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else{
	    ddate=(date+15) % 30;
	    cout<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;}
		fstream f;
		f.open("d:\\Fine.txt", ios::app);
		{
		f<<"This  book is issued :"<<b1<<"  to "<<std[b]<<endl; 
		f<<endl;
		f<<"             ****             "<<"Current Date is "<<date<<"/"<<month<<"/"<<year<<"              ****"<<endl;
		f<<endl;
		f<<"You must be re-issue or returned this book with in 15 days otherwise you  will  have to pay fine 1000 rupees!"<<endl;
		f<<endl;
		if (date<16)
		f<<"             ****             "<<"Your deadline is "<<date+15<<"/"<<month<<"/"<<year<<"              ****"<<endl;
	    else if(date>16 && month <12)
	    {
	    ddate=(date+15) % 30;
		f<<"             ****             "<<"Your deadline is  till  "<<ddate <<"/"<<month+1<<"/"<<year<<"              ****"<<endl;
		}
        else{
	    ddate=(date+15) % 30;
	    f<<"             ****             "<<"Your deadline is  till  "<<ddate<<"/"<<idate<<"/"<<year+1<<"              ****"<<endl;}
		
		f.close();	
		}
		cout<<endl<<endl;
		ofstream file2;
	    file2.open("d:\\Library_Books.txt", ios::trunc);
		file2<<"                                                             You  have issue  this  book :    "<<b1<<endl;
		file2<<"                                       ***                                                                           ***"<<endl;
		file2<<"                                                          -:            UPDATED  LIBRARY      :-       "<<endl;
		file2<<"                                       ***                                                                           ***"<<endl;
		file2<<endl;
		cout<<endl;
		for (int q=0;q<30;q++){
	    if (common[q] == b1)
		{b = q;
			common[q]="This Book  is Issued";
			}
		file2<<common[q]<<endl;} 
		cout<<endl<<endl;
		cout<<"IF you want to add any new books in Library then type 'yes' !"<<endl;
		cin>>w;
		if(w  =="yes")
		{
		cout<<endl<<endl;
		cout<<"You can add  maximum 10 new books at a time!"<<endl;
		cout<<"How many books you want to enter? ";
		cin>>k;
		file2<<"                                       ***                                                                           ***"<<endl;
	for (int j=30;j<30+k;j++)
	{
	
		cout<<"Enter new book :";
		cin>>common[j];
		cout<<endl;
		file2<<common[j]<<endl;
	}
	file2.close();
}
	exit(-1);
	}
}  
};
int main()
{
	int a;
	string b;
	Department_1 d1;
	Department_2 d2;
	Department_3 d3;
	Department_4 d4;
	Department_5 d5;
	software_section s2;
	manager ma;
	student s1;
	Database_Library dl;
	librarian l;
	s1.input3();
	cout<<endl;
	cout<<"If you want to  go  Software  section  then   type  'YES' ,  otherwise  it will show you Library bookS !"<<endl;
	cin>>b;
	if(b=="yes")
	s2.ss1();
	else{
	dl. Library_books();
	dl. Library_books123();
	s2.ss();
	d1.computer_sc();
	d2.electrical_eng();
	d3.medical();
	d4. aviation_man();
	d5.mass_com();
	l.input3();
	ma.manager1();
	cout<<endl<<endl<<endl;
	cout<<"Now  there  are  five  departments  and  its   your choice  in   which   department  you   want  to  Go!"<<endl;
	cout<<endl<<endl;
	cout<<"For entering Computer science Department then type  : 1 "<<endl;
	cout<<endl;
	cout<<"For entering Electrical Enginnering Department then type : 2 "<<endl;
	cout<<endl;
	cout<<"For entering Mediacl Department then type  : 3 "<<endl;
	cout<<endl;
	cout<<"For entering Aviation Management Department then type  : 4 "<<endl;
	cout<<endl;
	cout<<"For entering Mass Communication Department then tupe : 5 "<<endl;
	cout<<endl;
	cin>>a;
	if (a==1)
	{d1.computer_sc1();}
	else if(a==2)
	{d2.electrical_eng1();}
	else if(a==3)
	{d3.medical1();}
	else if(a==4)
	{d4.aviation_man1();}
	else if(a==5)
	{d5.mass_com1();}
	else
	cout<<"You enter invalid number ";}
	return 0;
}
