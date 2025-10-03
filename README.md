# Restaurant-bill
    #include <stdio.h>

    int main() {
    char customerName[50];
    int tableNumber, quantity;
    const float pricePerBurger = 5.00;
    float subtotal, tax, total;

    printf("Enter Customer Name (no spaces): ");
    scanf("%s", customerName);

    printf("Enter Table Number: ");
    scanf("%d", &tableNumber);

    printf("Enter quantity of Burger ($5.00 each): ");
    scanf("%d", &quantity);

    subtotal = quantity * pricePerBurger;
    tax = subtotal * 0.07; // 7% tax
    total = subtotal + tax;

    printf("\n----- RESTAURANT BILL -----\n");
    printf("Customer Name: %s\n", customerName);
    printf("Table Number : %d\n", tableNumber);
    printf("Item         Qty   Price\n");
    printf("-------------------------\n");
    printf("Burger        %2d   $%.2f\n", quantity, subtotal);
    printf("-------------------------\n");
    printf("Subtotal          $%.2f\n", subtotal);
    printf("Tax (7%%)          $%.2f\n", tax);
    printf("Total Amount      $%.2f\n", total);
    printf("-------------------------\n");
    printf("Thank you!\n");

    return 0;
    }

