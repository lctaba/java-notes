- 找出项目中所有的切点。
- 切面也是一个bean。
- 找出所有切面类型的bean找出来，然后把切点都保存起来。
- 然后创建bean对象的时候去缓存查找该bean创建的时候需不需要增强。
- 需要增强就对其进行增强，用动态代理。





