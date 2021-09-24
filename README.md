import pytest

def test_list_methods():
    numbers = ['1', '2', '3', '4', '5', '6', '7']
    numbers.append('8')
    assert numbers == ['1', '2', '3', '4', '5', '6', '7', '8']
    numbers.remove('8')
    assert numbers == ['1', '2', '3', '4', '5', '6', '7']
    assert numbers.index('1') == 0
    assert numbers.index('2') == 1
    numbers_copy = numbers.copy()
    assert numbers_copy == ['1', '2', '3', '4', '5', '6', '7', '8']
    
   
def test_dictionary():
   
    numbers_dictionary = {
        'one': '1',
        'two': '2',
        'three': '3',
    }
    assert numbers_dictionary['two'] == '2'
    assert 'two' in numbers_dictionary
    numbers_dictionary['four'] = '4'
    assert numbers_dictionary['four'] == '4'
    
