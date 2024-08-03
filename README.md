# count-of-rats
def food_sufficiency(r, unit, arr):
    
    if arr is None:
        return -1


    total_food_required = r * unit

    
    total_food_available = sum(arr)


    if total_food_available < total_food_required:
        return 0
    
    return total_food_available

r = 7
unit = 2
arr = [2, 8, 3, 5, 7, 4, 1, 2]
print(food_sufficiency(r, unit, arr))  
