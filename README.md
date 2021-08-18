#include<iostream>
int main(){
  int gryf = 0;
  int huff = 0;
  int raven = 0;
  int slyth = 0;

int answer1;
int answer2;
int answer3;
int answer4;

std::cout << "============================\n";
std::cout << "You have started sorting hat quiz!\n";
std::cout << "============================\n\n";


std::cout << "Q1) When I'm dead, I want people to remember me as:\n1) The Good\n2) The Great\n3) The Wise\n4) The Bold\n";

std::cin >> answer1;
if(answer1 == 1){
  huff = huff + 1;
}
else if(answer1 == 2){
  slyth = slyth + 1;
}
else if( answer1 == 3){
  raven = raven + 1;
}
else if( answer1 ==4){
  gryf = gryf + 1;
}
else{
  std::cout << "Invalid Point\n";
}

std::cout << "=============================\n";
std::cout << "Q2) Dawn or Dusk?\n1) Dawn\n2) Dusk\n";

std::cin >> answer2;

if(answer2 == 1)
{
  gryf = gryf + 1;
  raven = raven + 1;
}
else if(answer2 == 2){
    huff = huff + 1;
    slyth = slyth + 1;
}
else{
  std::cout << "Invalid Point\n";
}

std::cout << "=============================\n";
std::cout << "Q3) Which kind of instrument most pleases your ear?\n1) The violin \n2) The trumpet\n3) The piano\n4) The drum\n";

std::cin >> answer3;

if(answer3 == 1){
   slyth = slyth + 1;
}
else if(answer3 == 2){
  huff = huff + 1;
}
else if(answer3 == 3){
  raven  = raven + 1;
}
else if(answer3 == 4){
  gryf = gryf + 1;
}
else{
  std::cout << "Invalid Point\n";
}

std::cout << "=============================\n";
std::cout << "Q4) Which road tempts you most?\n1) The wide, sunny grassy lane \n2) The narrow, dark, lantern-lit alley\n3) The twisting, leaf-strewn path through woods\n4) The cobbled street lined (ancient buildings)\n";


std::cin >> answer4;

if(answer4 == 1){
  huff = huff + 1;
}
else if(answer4 == 2){
  slyth = slyth + 1;
}
else if(answer4 == 3){
  gryf = gryf + 1;
}
else if(answer4 == 4){
  raven = raven + 1;
}
else{
  std::cout << "Invalid point\n";
}

std::string house;
int max = 0;

if(gryf > max){
  max = gryf;
  house = "Gryffindor";
}
else if(huff > max){
  max = huff;
  house = "Hufflepuff";
}
else if(raven > max){
  max = raven;
  house = "RavenClaw";
}
else if(slyth > max){
  max = slyth;
  house = "Hufflepuff";
}
else{
  std::cout << "Its Impossible\n";
}

std::cout <<"=============================\n";
std::cout << "You Belong to: " << house <<"\n";

}
