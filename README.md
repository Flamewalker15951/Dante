int[] nums = { 7, 2, 9 ,4 ,1, 0};

// сортировка
int temp;
for (int i = 0; i < nums.Length - 1; i++){
    for (int j = i + 1; j < nums.Length; j++){
        if (nums[i] > nums[j]){
            temp = nums[i];
            nums[i] = nums[j];
            nums[j] = temp;
        }
    }
}

// вывод
Console.WriteLine("Вывод отсортированного массива");
for (int i = 0; i < nums.Length; i++) {
    Console.WriteLine(nums[i]);
}
