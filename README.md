def calculate_total_cost(items, discount_rate):
    """Calculates the total cost of a list of items after applying a discount.""" 
    total_price = 0
    for item in items:
        total_price += item.price  # Accumulate price of each item
        
    discounted_price = total_price * (1 - discount_rate)  # Apply discount
    
    return discounted_price 

# Example usage:
item_list = [
    {"name": "Shirt", "price": 20}, 
    {"name": "Pants", "price": 30} 
]
discount = 0.1  # 10% discount
final_cost = calculate_total_cost(item_list, discount)
print(f"Total cost with discount: {final_cost}")
