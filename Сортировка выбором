#include <iostream>
#include <vector>
#include <algorithm>

void selection_sort(std::vector<int>& arr) {
    // Проходим по всем элементам массива
    for (size_t i = 0; i < arr.size(); ++i) {
        // Предполагаем, что первый элемент - минимальный
        size_t min_index = i;

        // Ищем минимальный элемент в оставшейся части массива
        for (size_t j = i + 1; j < arr.size(); ++j) {
            if (arr[j] < arr[min_index]) {
                min_index = j;
            }
        }

        // Меняем найденный минимальный элемент с первым элементом в неотсортированной части
        std::swap(arr[i], arr[min_index]);
    }
}

int main() {
    // Создаем тестовый массив
    std::vector<int> test_array = {64, 25, 12, 22, 11};
    std::cout << "Исходный массив: ";
    for (int num : test_array) {
        std::cout << num << " ";
    }
    std::cout << std::endl;

    // Сортируем массив
    selection_sort(test_array);

    std::cout << "Отсортированный массив: ";
    for (int num : test_array) {
        std::cout << num << " ";
    }
    std::cout << std::endl;

    return 0;
}
