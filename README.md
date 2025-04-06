def split_comma(string):
    split_list = string.split(',')
    return {
        'first_half': split_list[0],
        'second_half':split_list[1]
        }

        

if __name__ == '__main__':
    my_dictionary = {
        'fav_food': 'yogurt',
        'fav_sport': 'football',
        'fav_day': 'friday'
        }
    for element in my_dictionary:
        print (element)
        print(my_dictionary[element])
        
    logs = 'wdjhbsDSBVIBSDVIBihdbiygasibiydgfhducyvsdjgvuygdsc'
    logs_count = {}
    alpha = 'abcdefghijklmnopqrstuvwxyz'
    for letter in alpha:
        for char in logs:
            if char == letter :
                if char in logs_count:
                    logs_count[char]+=1
                else:
                    logs_count[char] = 1
                
    for key, value in logs_count.items():
        output = '{},{}\n'.format(key, value)
        print(output)
        
    halves = split_comma('tomato, carrot')
    print(halves)# dictionaries-intro
