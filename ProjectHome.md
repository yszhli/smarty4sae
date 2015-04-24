smarty3.0 rc3 for sina app engine

在sae上demo地址: http://26.cakephp.sinaapp.com/demo/



主要说明：
> 模板编译后的缓存文件，使用memcache缓存保存。

> 缓存有效时间由memcache缓存的保存时间，所设置的smarty缓存时间共同决定。

> 修改模板文件时，缓存文件自动更新。

使用方法：

> $smarty->compile\_dir = 'saemc://smartytpl/';

> $smarty->cache\_dir = 'saemc://smartytpl/';

> $smarty->compile\_locking = false;

> 此三行必需，设置smarty的三个变量。其中两个dir中的smartytpl可修改，但必须以saemc://开始


配置要求：
> 需要在sae管理面板开启memcache缓存

smarty修改记录
> 见wiki中，修改行数不足10行，最大程度保证了smarty的原汁原味