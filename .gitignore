class Solution {
    public void merge(int[] nums1, int m, int[] nums2, int n) {
        // nums1'in sonundan başlayarak birleştirme işlemi yapılır
        int i = m - 1; // nums1'in son geçerli elemanının indeksi
        int j = n - 1; // nums2'nin son elemanının indeksi
        int k = m + n - 1; // nums1'in toplam uzunluğunun sonundan başlama noktası

        // Her iki diziyi karşılaştırarak birleştirme
        while (i >= 0 && j >= 0) {
            if (nums1[i] > nums2[j]) {
                nums1[k] = nums1[i];
                i--;
            } else {
                nums1[k] = nums2[j];
                j--;
            }
            k--;
        }

        // Eğer nums2'de eleman kaldıysa (nums1 zaten yerinde)
        while (j >= 0) {
            nums1[k] = nums2[j];
            j--;
            k--;
        }
    }

    public static void main(String[] args) {
        Solution solution = new Solution();
        int[] nums1 = {1, 2, 3, 0, 0, 0}; // Uzunluk m + n
        int m = 3;
        int[] nums2 = {2, 5, 6};
        int n = 3;

        solution.merge(nums1, m, nums2, n);

        // Sonucu yazdır
        for (int num : nums1) {
            System.out.print(num + " ");
        }
    }
}
