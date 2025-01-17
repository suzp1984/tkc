2022/06/25
  * 完善 platform_prepare

2022/06/20
  * 增加 log\_if\_fail。

2022/06/17
  * 完善str_unescape

2022/06/12
  * conf doc 支持向数组中追加数据。 

2022/06/07
  * 完善fscript调试器(感谢兆坤提供补丁)。

2022/06/04
  * 增加函数 conf\_doc\_set\_node\_prop 

2022/06/03
  * 增加函数 conf\_doc\_node\_dup

2022/05/31
  * 增加函数str\_encode\_xml\_entity/str\_encode\_xml\_entity\_with\_len。
  * 增加conf\_xml用于读写xml文件。  

2022/05/27
  * 增加函数tk\_replace\_char
  * typed\_array支持bool类型(感谢兆坤提供补丁)。
  * 去除debugger警告log (感谢兆坤提供补丁)。
  * 增加debugger\_client分发其他消息处理(感谢兆坤提供补丁)。

2022/05/26
  * 增加函数tokenizer\_next\_str，用于解析带引号的字符串。
  * 完善func\_call\_parser，支持带引号的参数。

2022/05/25
  * 完善编辑脚本（感谢朝泽提供补丁）
    * scons -c时不执行app_helper的prepare()
    * 修复项目编译时由于awtk的idl.json不存在导致idl_gen失败的问题

2022/05/20
  * 增加EMITTER\_ENABLE/EMITTER\_DISABLE

2022/05/19
  * 完善func\_json\_save\_ex（感谢国文提供补丁）。
  * 增加函数tk_memdup
  * 增加fscript函数binary
  * 完善func\_str

2022/05/18
  * 完善Windows下utf8转换。按照utf16的规则，对大于0x10000的字符值进行正确的编码 (感谢俊圣提供补丁)

2022/05/16
  * 完善 utf16\_to\_utf8  拷贝不下, 返回NULL,  避免崩溃或越界访问(感谢俊圣提供补丁)
  * 完善 tk\_utf8\_dup\_utf16 (感谢俊圣提供补丁)

2022/05/13
  * 修复 fscript中json\_load参数个数大于1时的问题（感谢国文提供补丁）。

2022/05/11
  * 完善 conf\_obj\_save

2022/05/02
  * 增加 tk\_object\_copy\_props。

2022/04/26
  * 完善 stream serial 的文档（感谢智明提供补丁）。

2022/04/24
  * 增加 weak 机制以及在 g2d 和 raw 中增加 weak （感谢智明提供补丁）。

2022/04/23
  * 完善 socket\_resolve 防止溢出（感谢叶冬提供补丁）
  * 完善 tk\_socket\_close 支持 AWorks（感谢叶冬提供补丁）
  * 增加 async\_call\_init\_ex2（感谢叶冬提供补丁）

2022/04/22
  * 增加 tk\_eval\_ratio\_or\_px
  * 增加 TK\_STR\_IS\_EMPTY
  * 增加 TK\_STR\_IS\_NOT\_EMPTY
  * 完善 idl_gen（感谢王程提供补丁）。

2022/04/19
  * 完善 tk\_istream\_read\_line

2022/04/18
  * 增加函数 path\_app\_root\_ex
  * awtk 修复缺少连接 ws2_32 类库的问题 （感谢智明提供补丁）。
  
2022/04/16
  * 增加函数 tk\_socket\_bind\_ex
  * 增加函数 tk\_iostream\_udp\_create\_client\_ex

2022/04/14
  * 让 windows 的串口也支持 select 的形式（感谢智明提供补丁）。

2022/04/09
  * fscript 增加 define\_param 用于辅助反向生成 AWBlock。
  * 完善 fscript 语法检查

2022/04/07
  * 增加函数 url\_to\_string。

2022/04/01
  * 完善 URL 解析并增加一些新的 schema。
  * 完善 ubjson writer

2022/03/31
  * 增加带统计功能的 stream （感谢林福提供）
  * 增加移除和替换 qaction 的 action\_darray\_thread（感谢林福提供）

2022/03/30
  * fscript 支持延迟解析函数。
  * 完善 fscript 局部变量的访问。
  * fscript 支持通过 require 函数加载模块。

2022/03/29
  * 优化 fscript 局部变量的访问。
  * 更新 aworkslp 移植代码（感谢文静提供）
  * 删除 mingw 的 UNICODE 宏和 msvc 统一宏的版本（感谢智明提供补丁）。

2022/03/28
  * 完善 fscript。

2022/03/23
  * 改用 mingw 默认的宏来定义 MINGW 宏（感谢智明提供补丁）。
  * 完善 ubjson 对字符的处理（感谢攀峰提供补丁）

2022/03/22
  * 完善 mingw 编译（感谢智明提供补丁）。

2022/03/21
  * 完善 mingw 编译（感谢智明提供补丁）。

2022/03/20
  * 完善 ubjson\_writer\_write\_object。
  * 完善 fscript 函数 len

2022/03/19
  * 完善 fscript 函数 bit\_not
  * 完善 fargs\_get\_data\_and\_size
  * 完善 object\_date\_time 支持 foreach。

2022/03/18
  * 完善 tk_\cond\_var\_wait（感谢兆坤提供补丁）。

2022/03/16
  * 增加通配符匹配函数 tk\_wild\_card\_match。

2022/03/10
  * 完善 fscript debugger

2022/03/04
  * 修改 csv 中的内存泄漏（感谢林福提供补丁）。

2022/03/02
  * AWorks 的 serial\_helper 增加设置超时的接口（感谢林福提供补丁）。

2022/02/24
  * 增加函数 str\_format/str\_append\_format。

2022/02/23
  * 修复导出 IDL 文件的时候因为查找不到依赖的类导致出现警告（感谢智明提供补丁）。
  * 集成了 IoT.js，所以同步更新 app\_helper\_base.py（感谢朝泽提供补丁）
  * 修复编译警告（感谢智明提供补丁）。

2022/02/22
  * 完善 fscript 调试器。

2022/02/21
  * 修复 fscript global 对象初始化的问题。
  * 修复 value\_int64/value\_uint64 对大数的处理。

2022/02/18
  * 增加函数 fscript\_set\_global\_object。

2022/02/15
  * conf 对象支持 foreach\_prop。
  * conf 支持创建子对象。

2022/02/10
  * 完善 API 注释（感谢朝泽提供补丁）
  * 完善 str\_append\_json\_str。

2022/02/04
  * 增加函数 path\_basename\_ex。

2022/02/02
  * 完善 fscript 语法错误检查。

2022/01/29
  * 完善 fscript debugger

2022/01/24
  * 优化 tk\_strncpy（感谢智明提供补丁）
  * 完善 fscript debugger

2022/01/23
  * 完善 fscript debugger, 支持 attach/launch 两种启动方式。

2022/01/22
  * 完善 fscript debugger

2022/01/21
  * 完善 fscript debugger 并增加 fdb 命令行调试工具。
  * 完善 aworks 平台的 serial\_helper.c（感谢文静提供）

2022/01/20
  * 增加 fscript 的构造函数和析构函数（感谢智明提供补丁）

2022/01/19
  * 完善 fscript 调试器（支持 step in/step out/step over/reload code)。

2022/01/16
  * 完善 fscript 支持调试器。

2022/01/13
  * 优化 tk\_object\_get\_child\_object（感谢雨欣提供补丁）

2022/01/11
  * 修复 WITHOUT\_FSCRIPT 没有生效的问题。
  * 完善 fscript 表达式。

2022/01/10
  * 完善 fscript if/elseif/else 语句
  
2022/01/08
  * fscript 的 log 函数改名为 logf，避免与 flow 中的 log 重名。
  * fscript 增加 date\_time\_get\_prop/date\_time\_set\_prop 等函数。 

2022/01/07
  * fscript 增加 str\_is\_empty/str\_len/array\_is\_empty/array\_size 等函数。
  * object\_typed\_array 支持通过 TK\_OBJECT\_PROP\_SIZE 获取元素个数。
  * object\_typed\_array 支持通过 set\_prop/get\_prop 访问元素。
  * fscript 支持 for/for\_in 语句。

2022/01/06
  * fscript 增加 random0to1。
  * fscript 支持 until/repeat_times/repeat 语句。
  * fscript 中增加 is\_int/is\_odd/is\_even 等函数

2022/01/05
  * fscript 公开函数 value\_id/value\_func。
  * fscript 增加 log10/pow10 等函数。
  * 修复注释错误（感谢朝泽提供补丁）
  * fscript 中三角函数增加以度数为单位的相应函数。

2022/01/04
  * fscript 支持保存函数名，方便调试。

2022/01/02
  * 修复 emitter 被覆盖的问题（感谢智明提供补丁）
  * 修复 fscript 中 while 语句对 return 的处理。

2022/01/01
  * 优化 fscript 函数调用。
  * 公开结构 fscript\_func\_call\_t。
  * fscript 支持设置错误处理函数。
  * fscript 增加函数 sleep\_ms。

2021/12/31
  * fscript 允许重载 print 函数。
  * 修复 emitter 的事件中删除事件同时递归触发事件导致 emitter 不正常的问题（感谢 zxc3489 和智明提供补丁）
  * 修复使用 thread\_with\_pthread 时，线程运行完毕后调 用 join 函数出现内存泄漏的问题 （感谢雨欣提供补丁）
  * fscript 去掉 a,b,c,d 快速变量，a,b,c,d 和普通变量一样处理。

2021/12/29
  * 修复 fscript 中 unset 的问题。
  * fscript 增加 f64/double 数据类型转换函数。

2021/12/28
  * 完善 serial\_helper.c（感谢朝泽提供补丁）

2021/12/26
  * 增加函数 array\_reverse
  * 增加 fscript 函数 array\_reverse

2021/12/25
  * 增加函数 str\_reverse/str\_count。
  * 增加 fscript 函数 text\_reverse/text\_count。

2021/12/24
  * 增加状态机（感谢林福提供补丁）
  * 修复单元测试：兼容非 utf8 编码的编译器（VS2015）（感谢雨欣提供补丁）
  * 完善部分 cast 函数的文档。

2021/12/23
  * 增加 aworkslp 平台支持（感谢林福提供补丁）
  * fscript 增加 code\_id，方便以后支持调试。
  * 编译嵌入式 linux 不使用 WITH\_SDL 宏，以及中文编码问题（感谢陈谭提供补丁）
  * 修正 Win32 串口操作速度被限制的问题（感谢陈谭提供补丁）

2021/12/22
  * 复原被覆盖的 tools/idl\_gen/README.md（感谢雨欣提供补丁）
  * 增加 tkc/sha256.h

2021/12/20
  * fscript 支持全局对象。

2021/12/11
  * 增加 tk\_str\_is\_in\_array。
  * 增加 tk\_utf8\_trim\_invalid\_char。

2021/12/09
  * 完善 json 解析对整数的处理。

2021/12/02
  * TKC 从 AWTK 中独立出来。
  * 重构编译脚本，增加 awtk\_config\_common.py。
  * 一些可能重名函数增加 tk_前缀。

2021/12/06
  * 支持 linux 系统交叉编译（感谢智明提供补丁）。
