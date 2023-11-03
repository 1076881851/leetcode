
//一般做法
func getModifiedArray(length int, updates [][]int) []int {
    array := make([]int, length)
    for _, update := range updates {
        for i := update[0]; i <= update[1]; i++ {
            array[i] += update[2]
        }
    }
    return array
}



