# Homework-8
#include <stdio.h>

char to_lower (char a ){
  if(a >= 'A' && a <= 'Z'){
    return a | 32;    
  }

  return a;

}

char to_upper(char c){
  if(c>='a'&& c<= 'z'){
    return c & ~32;    
  }
  return c;
}

int main (){
  char input  = 'A' ;
  char input1 = 'a';
  char output1 = to_upper(input);
  char output = to_lower(input);
  printf("Input:%c,Output:%c,Input1:%c,Output1:%c\n",input ,output,input1,output1);
  return 0;
}
