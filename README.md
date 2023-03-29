# The following code sorts an array in descending order using the bubble sort algorithm. It iterates through the array and compares each element to the one next to it. If the number on the left is greater than the number on the right, the two elements are swapped. This process is repeated until the array is sorted in descending order. The conditional part of the code ensures that the algorithm will only sort even numbers. The bubble sort algorithm has a time complexity of O(n^2). 

# Conditional bubble sort (only odd numbers)
def conditional_bubble_sort(list_of_numbers):
    for i in range(len(list_of_numbers)):
        for j in range(len(list_of_numbers) - 1):
            if list_of_numbers[j] > list_of_numbers[j + 1] and check_if_even(list_of_numbers[j]) == False:
                list_of_numbers[j], list_of_numbers[j + 1] = list_of_numbers[j + 1], list_of_numbers[j]
    return list_of_numbers 