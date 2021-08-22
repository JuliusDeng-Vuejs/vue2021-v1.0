# 1 vue组件文件的style里面，通常写上scoped，限制在所有组件用到同一个类名

# 2 vue组件文件的script里面写上name："xxx",

# 3 props传值时要不要加v-bind:,  v-bind:后面是一个表达式，而表达式会返回一个结果， 如果不加v-bind:,那么props传的就是一个字符串！
#   props传递的值是只读的，不允许修改！