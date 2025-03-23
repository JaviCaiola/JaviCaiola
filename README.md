![imagen github optimizada](https://github.com/JaviCaiola/JaviCaiola/assets/114126710/61888a1d-6ad4-4981-b80d-5a92b44bf17d)

# Hola  (•◡•) / 👋

#### Desarrollador web Full Stack 🧰
#### FrameWorks: Spring Boot, Angular, Node.js 
#### En busca de proyectos interesantes los cuales realizar, y siempre a disposicion para colaborar juntos, no dudes en contactar!
#### 
####
####
####

#include<stdio.h>
#include<unistd.h>
#include<pthread.h>

void *thread_function(void *arg);
int i, j;

int main() {
    pthread_t a_thread; // declaración de hilo
    pthread_create(&a_thread, NULL, thread_function, NULL); // se crea el subproceso
    pthread_join(a_thread, NULL); // el proceso espera a que finalice el subproceso. Comente esta línea para ver la diferencia

    printf("Dentro del programa principal imprimimos números pares\n");
    for(j = 0; j < 50; j++) {
        if (j % 2 == 0) {
            printf("%d\n", j);
        }
        sleep(1);
    }
    return 0;
}

void *thread_function(void *arg) {
    // el trabajo que debe realizar el hilo se define en esta función
    printf("Dentro del hilo imprimimos números impares\n");
    for(i = 0; i < 50; i++) {
        if(i % 2 > 0) {
            printf("%d\n", i);
        }
        sleep(1);
    }
    return NULL;
}
