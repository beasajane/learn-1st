* flex-grow
  The flex-grow CSS property sets the flex grow factor of a flex item's main size.
  比如剩余空间为 x，三个元素的 flex-grow 分别为 a，b，c。设 sum 为 a + b + c。那么三个元素将得到剩余空间分别是
  如果sum >= 1 那么剩余空间分别为 x * a / sum, x * b / sum, x * c / sum。
  如果sum <= 1 那么剩余空间分别为 (x*sum) * a / sum, (x*sum) * b / sum, (x*sum) * c / sum。
* flex-shrink
  每个flex item收缩的空间为：item的宽度 * flex-shrink系数/ 总权重TW * 需要收缩的总宽度
  先计算总权重TW = item(1)的宽度 * flex-shrink(1) + item的宽度(2) *flex-shrink(2) + item的宽度(3) *flex-shrink(3)main-axis