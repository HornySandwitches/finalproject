#include <stdio.h>

int main() 
{
    char name[50];
    int phone_number;
    int customer_id;

    int body_soap;
    int hair_cream;
    int hair_spray;
    int body_spray;

    int sugar;
    int tea;
    int coffee;
    int rice;
    int wheat;

    int cola_next;
    int water;
    int juice;
    int mojitos;
    int pakola;

    int total;
    int cosmetics_total = 0;
    int grocery_total = 0;
    int beverage_total = 0;


    printf("\n---------------------");
    printf("\n*Welcome to TSAY MART*");
    printf("\n---------------------");
    printf("\nBILLING SYSTEM");
    printf("\n----------------------\n");
    printf("Customer Details\n\n");
    
        printf("------------- PROMOTIONS -------------\n");
    printf("1. Buy 2 Cola Next, Get 1 Cola Next Free\n");
    printf("2. Buy 2 Body Spray, Get 1 Body Spray Free\n");
    printf("3. Buy 2 Coffee, Get 1 Coffee Free\n");
    printf("--------------------------------------\n");

    printf("Customer Name: ");
    scanf("%s", name);

    printf("Customer Number: ");
    scanf("%d", &phone_number);

    printf("Customer ID: ");
    scanf("%d", &customer_id);

    printf("-----------------------\n");

    printf("COSMETICS\n\n");

    printf("Body Soap (pkr 50) : ");
    scanf("%d", &body_soap);

    printf("Hair Cream (pkr 200) : ");
    scanf("%d", &hair_cream);

    printf("Body Spray (pkr 300) : ");
    scanf("%d", &body_spray);
    
    
    if (body_spray >= 2) {
        printf("Promotion Applied: Buy 2 Body Spray, Get 1 Body Spray Free\n");
        body_spray -= 1;
    }

    printf("Hair Spray (pkr 300) : ");
    scanf("%d", &hair_spray);

    int boso = 50 * body_soap;
    int hc = 200 * hair_cream;
    int hs = 300 * hair_spray;
    int bosp = 300 * body_spray;

    cosmetics_total = boso + hc + hs + bosp;

    printf("Body soap : %d pkr\n", boso);
    printf("Hair Cream : %d pkr\n", hc);
    printf("Hair Spray : %d pkr\n", hs);
    printf("Body Spray : %d pkr\n", bosp);
    printf("Total Cosmetic Price : %d pkr\n", cosmetics_total);

    printf("-----------------------\n");

    
    printf("GROCERIES\n\n");

    printf("Sugar (pkr 100) : ");
    scanf("%d", &sugar);

    printf("Tea (pkr 50) : ");
    scanf("%d", &tea);

    printf("Coffee (pkr 100) : ");
    scanf("%d", &coffee);

    
    if (coffee >= 2) {
        printf("Promotion Applied: Buy 2 Coffee, Get 1 Coffee Free\n");
        coffee -= 1;
    }

    printf("Rice (pkr 100) : ");
    scanf("%d", &rice);

    printf("Wheat (pkr 100) : ");
    scanf("%d", &wheat);

    int s = 100 * sugar;
    int t = 50 * tea;
    int c = 100 * coffee;
    int r = 100 * rice;
    int w = 150 * wheat;

    grocery_total = s + t + c + r + w;

    printf("Sugar : %d pkr\n", s);
    printf("Tea : %d pkr\n", t);
    printf("Coffee : %d pkr\n", c);
    printf("Rice : %d pkr\n", r);
    printf("Total Grocery Price : %d pkr\n", grocery_total);

    printf("-----------------------\n");

    
    printf("BEVERAGES\n");

    printf("Cola Next (pkr 100) : ");
    scanf("%d", &cola_next);

    
    if (cola_next >= 2) {
        printf("Promotion Applied: Buy 2 Pepsi, Get 1 Pepsi Free\n");
        cola_next -= 1;
    }

    printf("Water (pkr 100) : ");
    scanf("%d", &water);

    printf("Juice (pkr 100) : ");
    scanf("%d", &juice);

    printf("Mojitos (pkr 150) : ");
    scanf("%d", &mojitos);

    printf("Pakola (pkr 100) : ");
    scanf("%d", &pakola);

    int cn = 100 * cola_next;
    int wa = 100 * water;
    int ju = 100 * juice;
    int moj = 150 * mojitos;
    int pak = 100 * pakola;

    beverage_total = cn + wa + ju + moj + pak;

    printf("Cola Next : %d pkr\n", cn);
    printf("Water : %d pkr\n", wa);
    printf("Juice : %d pkr\n", ju);
    printf("Mojitos : %d pkr\n", moj);
    printf("Pakola : %d pkr\n", pak);
    printf("Total Beverage Price : %d pkr\n", beverage_total);

    printf("-----------------------\n");
    printf("Product name                                Quantity                                       Price\n\n");
	printf("Body Soap                                      %d                                             %d\n",body_soap,boso);
	printf("Hair Cream                                     %d                                             %d\n",hair_cream,hc);
	printf("Body Spray                                     %d                                             %d\n",body_spray,bosp);
	printf("Hair Spray                                     %d                                             %d\n",hair_spray,hs);
	printf("Suagr                                          %d                                             %d\n",sugar,s);
	printf("Tea                                            %d                                             %d\n",tea,t);
	printf("Coffee                                         %d                                             %d\n",coffee,c);
	printf("Rice                                           %d                                             %d\n",rice,r);
	printf("Wheat                                          %d                                             %d\n",wheat,w);
	printf("Pakola                                         %d                                             %d\n",pakola,pak);
	printf("Juice                                          %d                                             %d\n",juice,ju);
	printf("Cola Next                                      %d                                             %d\n",cola_next,cn);
	printf("Water                                          %d                                             %d\n",water,wa);
	printf("Mojitos                                        %d                                             %d\n",mojitos,moj);

    printf("-----------------------\n");
    
    total = cosmetics_total + grocery_total + beverage_total;

    printf("TSAY MART Checkout\n\n");
    printf("Customer Name : %s\n", name);
    printf("Customer Phone Number : %d\n", phone_number);
    printf("Customer ID : %d\n", customer_id);

    printf("Grocery Total Price : %d pkr\n", grocery_total);
    printf("Cosmetics Total Price : %d pkr\n", cosmetics_total);
    printf("Beverage Total Price : %d pkr\n", beverage_total);
    printf("Total Price : %d pkr\n", total);
    printf("--------------------------------------------------\n");

    return 0;
}
