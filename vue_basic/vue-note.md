# 1 computed 有缓存作用，而methods没有

# 2 v-else-if 比直接写 v-if效率更高：v-else-if是如果满足前面的条件就不会去判断后面的数据了，但直接都写v-if则不管是否以满足前面的条件都会去判断后面的数据
			
			<div v-if="n === 1">Angular</div>  // 若满足了n === 1 ，则不会看后面的这几个代码了
			<div v-else-if="n === 2">React</div>
			<div v-else-if="n === 3">Vue</div>
			
			<div v-if="n === 1">Angular</div>  // 即便满足了n === 1 ，也还是会看后面的这几个代码的
			<div v-if="n === 2">React</div>
			<div v-if="n === 3">Vue</div>
			
#		注：template不会增加页面结构，但只能与v-if 结合使用，不能与v-show结合使用（不生效）
	#		
	#		条件渲染：
							1.v-if
										写法：
												(1).v-if="表达式" 
												(2).v-else-if="表达式"
												(3).v-else="表达式"
										适用于：切换频率较低的场景。
										特点：不展示的DOM元素直接被移除。
										注意：v-if可以和:v-else-if、v-else一起使用，但要求结构不能被“打断”。

							2.v-show
										写法：v-show="表达式"
										适用于：切换频率较高的场景。
										特点：不展示的DOM元素未被移除，仅仅是使用样式隐藏掉
								
							3.备注：使用v-if的时，元素可能无法获取到，而使用v-show一定可以获取到。