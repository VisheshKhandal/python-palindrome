# python-palindrome
def is_palindrome(element):
  """Checks if a given element (string or number) is a palindrome."""
  return str(element) == str(element)[::-1]

def check_for_palindrome_list(data_list):
  """Checks if a list contains a palindrome (considering elements as individuals)."""
  for element in data_list:
    # Check if the element itself is a palindrome (string or number)
    if is_palindrome(element):
      return True
  return False

# Sample list (you can modify this list)
my_list = ["madam", "noon", "race", 121, "hello"]

# Check if the list contains a palindrome
if check_for_palindrome_list(my_list):
  print("The list contains a palindrome element.")
else:
  print("The list does not contain a palindrome element.")
