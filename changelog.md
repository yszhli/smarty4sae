#smarty3.0 rc3 for sae 修改记录

改动代码非常少，最大程度保留了smarty的原汁原味

# 代码修改记录 #


smarty\_internal\_templateparser.php

> $this->asp\_tags = false;// 替换ini\_get

smarty\_internal\_write\_file.php

> writeFile函数

> public static function writeFile($_filepath, $_contents, $smarty)

> {

> if (!file\_put\_contents($_filepath, $_contents)) {

> throw new Exception("unable to write file {$_filepath}");_

> return false;

> }

> return true;

> }