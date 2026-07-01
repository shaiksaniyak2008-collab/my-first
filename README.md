# my-first
def print_pattern(rows):
  current_num=1
  max_num=rows*(rows+1)
  width=len(str(max_num))+1
  for i in range(1,rows+1):
    row_str=""
    for j in range(i):
      row_str+=f"{current_num:>{width}}"
      current_num+=1
      total_width=rows+width
      print(row_str.rjust(total_width))
      print_pattern(4)
