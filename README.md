#include<stdio.h>
#include<string.h>

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
	int pakola;
	int juice;
	//int water;
	int chips;
	int thumbs_up;
	int total;
	int cosmetic_total;
	int grocery_total;
	int beverage_total;
	int total_grocery;
	
	
	
	printf("----------------\n");
	printf("BILLING SYSTEM\n");
	printf("--------------\n\n");
	printf("Customer Details\n\n");
	
	printf("Customer Name: ");
	scanf("%s", name);
	printf("Customer Number: ");
	scanf("%d",&phone_number);
	printf("Customer ID:");
	scanf("%d", &customer_id);
	
	printf("-----------------\n");
	
	printf("Cosmetics\n\n");
	
	printf("Body soap (Rs.100): ");
	scanf("%d",&body_soap);
	printf("Hair Cream (Rs.150): ");
	scanf("%d",&hair_cream);
	printf("Body spray (Rs200): ");
	scanf("%d", &body_spray);
	printf("Hair spray (Rs 140): ");
	scanf("%d",&hair_spray);
	
	printf("-----------------\n");
	
	printf("Groceries\n\n");
	
	printf("Sugar (Rs 40): ");
	scanf("%d", &sugar);
	printf("Tea (Rs20): ");
	scanf("%d", &tea);
	printf("Coffee (Rs 50): ");
	scanf("%d", &coffee);
	printf("Rice (Rs 170): ");
	scanf("%d", &rice);
	printf("Wheat (Rs 140): ");
	scanf("%d", &wheat);
	
	printf("-----------------\n");
	
	printf("BEVERAGES\n\n");
	
	printf("Pakola (Rs.70): ");
	scanf("%d", &pakola);
	printf("juice (Rs 50): ");
	scanf("%d", &juice);
	printf("Chips (Rs 40): ");
	scanf("%d", &chips);
	printf("Thumbs Up (Rs44): ");
	scanf("%d", &thumbs_up);
	
	printf("-----------------\n");
	
	int boso;
	int hc;
	int hs;
	int bosp;
	
	boso= 10* body_soap;
	hc = 25* hair_cream;
	hs= 50* hair_spray;
	bosp= 50* body_spray;
	cosmetic_total= boso + hc + hs + bosp;
	
	
	printf("Body soap: ");
	printf("%d Rs\n", boso);
	printf("Hair Cream: ");
	printf("%d Rs\n",hc);
	printf("Hair spray: ");
	printf("%d Rs\n");
	printf("Body Spray: ", hs);
	printf("%d Rs\n", bosp);
	printf("Total Cosmetic Price: ");
	printf("%d Rs\n", cosmetic_total);
	
	printf("-----------------\n");
	
	int s;
	int t;
	int c;
	int r;
	int w;
	
	s= 100 * sugar;
	t= 20 * tea;
	c = 50 * coffee;
	r= 170 * rice;
	w= 100 * wheat;
	grocery_total = s + t + c + r + w;
	
	printf("Sugar: ");
	printf("%d Rs\n",s);
	printf("Tea: ");
	printf("%d Rs\n",t);
	printf("Rice: ");
	printf("%d Rs\n",r);
	printf("Wheat: ");
	printf("%d Rs\n", w);
	printf("Total Grocery price: ", total_grocery);
	
	
	printf("-----------------\n");
	
	int pak;
	int ju;
	int ch;
	int thu;
	
	pak=70* pakola;
	ju= 50* juice;
	ch= 40* chips;
	thu= 44 * thumbs_up;
	beverage_total= pak+ju+ch+thu;
	
	printf("Pakola: ");
	printf("%d Rs\n", pak);
	printf("Juice: ");
	printf("%d Rs\n", ju);
	printf("Chips: ");
	printf("%d Rs\n", ch);
	printf("Thumbs up: ");
	printf("%d Rs\n", thu);
	printf("Total Beverage Price: ");
	printf("%d Rs\n", beverage_total);
	
	printf("-----------------\n");
	
	total= cosmetic_total + grocery_total + beverage_total;
	
	printf("Total Amount: ");
	printf("%d Rs\n", total);
	
	printf("-----------------\n");
	
	printf("Super Store Supermarket\n\n");
	
	printf("Customer Name: ");
	printf("%s\n", name);
	printf("Customer Number: ");
	printf("%d\n", phone_number);
	printf("Customer ID: ");
	printf("%d\n", customer_id);
	
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
	printf("Chips                                          %d                                             %d\n",chips,ch);
	printf("Thumbs up                                      %d                                             %d\n",thumbs_up,thu);
	
	
	printf("Gorcery Total Price: %d\n\n", grocery_total);
	
	printf("Cosmetic Total Price: %d\n\n", cosmetic_total);
	
	printf("Beverage Total Price: %d\n\n", beverage_total);
	
	printf("-----------------------------------------------------------------------------------------------------------------------------\n");
	
	return 0;
	
}
