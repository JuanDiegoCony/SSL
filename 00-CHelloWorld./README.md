El compilador seleccionado es el **gcc** (instalado a traves del MinGW).

La version del compilador gcc es **6.3.**

La version del lenguaje C es **C11**.

---------------------------------------

Para averiguar la versión del compilador puse gcc --version en la terminal. Luego para averiguar la version del lenguaje C use el siguiente codigo, que al ejecutarse me devolvio, "we are using C11":



  
  
  #include<stdio.h>
  
  
  int main() {

  
    if(__STDC_VERSION__  == 202000){
    
        
        printf("We are using C23!\n");
      
      
      }
    
    
    else if(__STDC_VERSION__ == 201710L){
    
      
      printf("We are using C17!\n");
    
    
    }
    
    
    else if (__STDC_VERSION__ == 201112L)
    
        
        printf("We are using C11!\n");
    
    
    return 0;
}
