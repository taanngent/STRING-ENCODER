#include <bits/stdc++.h>
#include<set>
using namespace std;
int x;int y;int key;int z;int a;int i;int p;int q;int flag;int e;int d;int n;int t;int u;
set<char> cset;
char strng[1000];int temp[50];char rsaen[1000];char keywrd[100];char alphabets[26];
char newalphabets[26];char enkstr[1000];string str;
void s1();void option();void workflow();void choose();void inputc();void enceaser();
void deceaser();void printc();void inputm();void enmatrix();int lengthm();void rsa();
int prime();void rsa_key();int minverse();void rsaencrypt();void rsadecrypt();int power();
void encryptdh();void decryptdh();void printdh();void dhkey();void inputdh();void keyarray();
void enkcipher();void dekcipher();void keywordcipher();
//Ceaser Cipher
void deceaser(){
i=0;
while(strng[i]!='\0'){
strng[i]=strng[i]-(key%26);
i++;
}
}
void enceaser(){
i=0;
while(strng[i]!='\0'){
strng[i]=strng[i]+(key%26);
i++;
}
system("cls");
cout<<"\n\n\n\n\t\t\t\tHURRAY NOW YOUR MESSAGE IS SAFE\n\n\n\n";
cout<<"\t\t\t-> TO SEE RESULT PRESS 1\n\n";
cout<<"\t\t\t-> TO ENCRYPT NEW MESSAGE PRESS 2\n\n\t\t\t";
cin>> a;
switch(a){
case 1:
system("cls");
cout<<"\n\n\n\n\t\t\tENCRYPTED MESSAGE IS : ";
printc();
deceaser();
cout<<"\n\n\t\t\tORIGINAL MESSAGE IS : ";
printc();
cout<<"\n\n\n\t\t\t-> TO ENCRYPT NEW MESSAGE PRESS 1\n\n\t\t\t";
cout<<"-> TO EXIT PRESS 2\n\n\t\t\t";
cin>>u;
switch(u){
case 1:
system("cls");
choose();
break;
case 2:
exit(0);
break;
default:
exit(0);
}
break;
case 2:
system("cls");
choose();
break;
default:
exit(0);
}
}
void inputc(){
cout<<"\n\n\n\n\n";
cout<<"\t\t\t-> ENTER MESSAGE HERE : ";
fflush(stdin);
cin.getline(strng, 1000);
cout<<"\n\n\t\t\t-> CHOOSE SECURITY KEY(integer) : ";
cin>> key;
system("cls");
}
void printc(){
i=0;
while(strng[i]!='\0'){
cout<<strng[i];
i++;
}
}
//===================================================================
//matrix method
//===================================================================
void inputm(){
cout<<"\n\n\n\n\n";
cout<<"\t\t\t-> ENTER MESSAGE HERE : ";
fflush(stdin);
cin.getline(strng, 1000);
system("cls");
}
int lengthm(){
i=0;
while(strng[i]!='\0')
i++;
return i;
}
void enmatrix(){
int l=lengthm();
p=sqrt(l)+1;
q=sqrt(l);
while(p*q<l)
p++;
char matrix[p][q];
for(int m=0;m<p;m++){
for(int n=0;n<q;n++){
matrix[m][n]=' ';
}
}
i=0;
for(int m=0;m<p;m++){
for(int n=0;n<q;n++){
if(strng[i]!='\0'){
matrix[m][n]=strng[i];
i++;
}
}
}
cout<<"\n\n\n\n\t\t\t\tHURRAY NOW YOUR MESSAGE IS SAFE\n\n\n\n";
cout<<"\t\t\t-> TO SEE RESULT PRESS 1\n\n";
cout<<"\t\t\t-> TO ENCRYPT NEW MESSAGE PRESS 2\n\n\t\t\t";
cin>> a;
switch(a){
case 1:
system("cls");
cout<<"\n\n\n\n\t\t\tENCRYPTED MESSAGE IS : ";
for(int m=0;m<q;m++){
for(int n=0;n<p;n++){
cout<< matrix[n][m];
}
}
cout<<"\n\n\t\t\tDECRYPTED MESSAGE IS : ";
for(int m=0;m<p;m++){
for(int n=0;n<q;n++){
cout<< matrix[m][n];
}
}
cout<<"\n\n\n\t\t\t-> TO ENCRYPT NEW MESSAGE PRESS 1\n\n\t\t\t";
cout<<"-> TO EXIT PRESS 2\n\n\t\t\t";
cin>>u;
switch(u){
case 1:
system("cls");
choose();
break;
case 2:
exit(0);
break;
default:
exit(0);
}
break;
case 2:
system("cls");
option();
break;
default:
exit(0);
}
}
//RSA ALGORITHM
int prime(int a){
y = sqrt(a);
for(i=2;i<=y;i++){
if(a%i==0)
return 0;
}
return 1;
}
int minverse(int a){
int c = 1;
while(1){
c = c + t;
if(c % a == 0)
return(c/a);
}
}
void rsa_key(){
int k=0;
e=0;d=0;
for(int s=2;s<t;s++){
if(t%s==0)
continue;
flag=prime(s);
if(flag==1 && s!=p && s!=q){
e=s;
flag= minverse(e);
if(flag>0){
d=flag;
k++;
}
}
if(e!=0&&d!=0)
break;
}
}
void rsaencrypt(){
key=e;
i=0;
while(strng[i]!='\0'){
if(strng[i]==' ')
rsaen[i]=' ';
else{
x=strng[i];
x=x-96;
z=1;
for(int j=0;j<key;j++){
z=z*x;
z=z%n;
}
temp[i]=z;
y=z+96;
rsaen[i]=y;
}
i++;
}
i=0;
cout<<"ENCRYPTED MESSAGE IS : ";
while(rsaen[i]!='\0'){
cout<<rsaen[i];
i++;
}
}
void rsadecrypt(){
key=d;
i=0;
char rsade[1000];
while(rsaen[i]!='\0'){
if(rsaen[i]==' ')
rsade[i]=' ';
else{
x=temp[i];
z=1;
for(int j=0;j<key;j++){
z=z*x;
z=z%n;
}
y=z+96;
rsade[i]=y;
}
i++;
}
i=0;
cout<<"DECRYPTED MESSAGE IS : ";
while((rsade[i]>96&&rsade[i]<123)||rsade[i]==' '){
cout<<rsade[i];
i++;
}
}
void rsa(){
cout<<"\n\n\n\n\n";
cout<<"\t\t\t-> ENTER FIRST PRIME NUMBER P : ";
cin>>p;
flag=prime(p);
if(flag==0){
cout<<"\n\n\t\t\tINVALID INPUT!!!!! REDIRECTING.............................";
i=0;
while(i<1000000000)
i++;
system("cls");
choose();
}
cout<<"\n\n\t\t\t-> ENTER SECOND PRIME NUMBER Q (P!=Q) : ";
cin>>q;
flag=prime(q);
if(flag==0||p==q){
cout<<"\n\n\t\t\tINVALID INPUT!!!!! REDIRECTING............................";
i=0;
while(i<1000000000)
i++;
system("cls");
choose();
}
n= p*q;
t= (p-1)*(q-1);
rsa_key();
cout<<"\n\n\n\n\t\t\t\t\tVALUE OF e : ";
cout<<e;
cout<<"\n\n\t\t\t\t\tVALUE OF d : ";
cout<<d;
cout<<"\n\n\n\t\t\tENTER THE MESSAGE : ";
fflush(stdin);
cin.getline(strng, 1000);
system("cls");
cout<<"\n\n\n\n\t\t\t\tHURRAY NOW YOUR MESSAGE IS SAFE\n\n\n\n";
cout<<"\t\t\t-> TO SEE RESULT PRESS 1\n\n";
cout<<"\t\t\t-> TO ENCRYPT NEW MESSAGE PRESS 2\n\n\t\t\t";
cin>> a;
switch(a){
case 1:
system("cls");
cout<<"\n\n\n\n\t\t\t";
rsaencrypt();
cout<<"\n\n\t\t\t";
rsadecrypt();
cout<<"\n\n\n\t\t\t-> TO ENCRYPT NEW MESSAGE PRESS 1\n\n\t\t\t";
cout<<"-> TO EXIT PRESS 2\n\n\t\t\t";
cin>>u;
switch(u){
case 1:
system("cls");
fflush(stdin);
choose();
break;
case 2:
exit(0);
break;
default:
exit(0);
}
break;
case 2:
system("cls");
option();
break;
default:
exit(0);
}
}
//KEYWORD CIPHER
void keyarray(char keywrd[100]){
for(i=97;i<123;i++){
alphabets[i-97]=i;
}
i=0;
x=0;
while(keywrd[i]!='\0'){
if(cset.find(keywrd[i])==cset.end()){
cset.insert(keywrd[i]);
newalphabets[x]=keywrd[i];
x++;
}
i++;
}
for(i=0;i<26;i++){
if(cset.find(alphabets[i])==cset.end()&&x<27){
cset.insert(alphabets[i]);
newalphabets[x]=alphabets[i];
x++;
}
}
}
void kinput(){
cout<<"\n\n\n\n\n";
cout<<"\t\t\t-> ENTER MESSAGE HERE : ";
fflush(stdin);
cin.getline(strng, 1000);
cout<<"\n\n\t\t\t-> CHOOSE KEYWORD(STRING) : ";
fflush(stdin);
cin.getline(keywrd, 100);
system("cls");
}
void keywordcipher(){
kinput();
keyarray(keywrd);
system("cls");
cout<<"\n\n\n\n\t\t\t\tHURRAY NOW YOUR MESSAGE IS SAFE\n\n\n\n";
cout<<"\t\t\t-> TO SEE RESULT PRESS 1\n\n";
cout<<"\t\t\t-> TO ENCRYPT NEW MESSSAGE PRESS 2\n\n\t\t\t";
cin>> a;
switch(a){
case 1:
system("cls");
cout<<"\n\n\n\n\t\t\tENCRYPTED MESSAGE IS : ";
enkcipher();
cout<<"\n\n\t\t\tORIGINAL MESSAGE IS : ";
dekcipher();
cout<<"\n\n\n\t\t\t-> TO ENCRYPT NEW MESSAGE PRESS 1\n\n\t\t\t";
cout<<"-> TO EXIT PRESS 2\n\n\t\t\t";
cin>>u;
switch(u){
case 1:
system("cls");
choose();
break;
case 2:
exit(0);
break;
default:
exit(0);
}
break;
case 2:
system("cls");
option();
break;
default:
exit(0);
}
}
void enkcipher(){
i=0;
while(strng[i]!='\0'){
if(strng[i]==' '){
enkstr[i]=' ';
}
else{
y=strng[i]-97;
enkstr[i]=newalphabets[y];
}
i++;
}
i=0;
while(enkstr[i]!='\0'){
cout<<enkstr[i];
i++;
}
}
void dekcipher(){
i=0;
char dekstr[1000];
int l=0;
while(enkstr[i]!='\0'){
if(enkstr[i]==' '){
dekstr[i]=' ';
}
else{
for(l=0;l<26;l++){
if(enkstr[i]==newalphabets[l]){
break;
}
}
dekstr[i]=alphabets[l];
}
i++;
}
i=0;
while(dekstr[i]!='\0'&&enkstr[i]!='\0'){
cout<<dekstr[i];
i++;
}
}
void choose(){
cout<<"\n\n\n\n";
cout<<"\t\t\t\tCHOOSE THE ENCRYPTION ALGORITHM\n\n\n\n";
cout<<"\t\t -> CEASER CIPHER ALGO PRESS 1\n\n";
cout<<"\t\t -> MATRIX METHOD ALGO PRESS 2\n\n";
cout<<"\t\t -> RSA ALGO PRESS 3\n\n";
cout<<"\t\t -> KEYWORD CIPHER ALGO PRESS 4\n\n";
cout<<"\n\t\t===============================================================\n\n";
cout<<"\n\t\t -> TO GO BACK TO MAIN MENU PRESS 5\n\n\t\t";
cin>> z;
system("cls");
switch(z){
case 1:
inputc();
enceaser();
break;
case 2:
inputm();
enmatrix();
break;
case 3:
rsa();
break;
case 4:
keywordcipher();
break;
case 5:
option();
break;
default :
exit(0);
}
}
void option(){
cout<<"\n\n\n\n\t\t\t\t\t\tMAIN MENU\n\n\n";
cout<<"\t\t\t -> TO PROCEED PRESS 1\n\n";
cout<<"\t\t\t -> TO EXIT PROGRAM PRESS 2\n\n";
cout<<"\t\t\t";
cin>> y;
system("cls");
switch(y){
case 1:
choose();
cout<<"\n\n";
break;
case 2:
exit(0);
break;
default:
exit(0);
}
}
int main(){
option();
return 0;
}
