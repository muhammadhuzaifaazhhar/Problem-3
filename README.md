# Problem-3
def compute_sales_stats(sales):
    commission_rate = 0.1 if sales > 100000 else 0.05
    commission = sales * commission_rate
    next_year_target = 0.05 * sales
    return commission, next_year_target

salesperson_name = input("Enter salesperson's last name: ")
sales = float(input("Enter sales: "))

commission, next_year_target = compute_sales_stats(sales)

print(f"Salesperson Name: {salesperson_name}")
print(f"Commission: {commission}")
print(f"Next Year's Target: {next_year_target}")
