# DevRandomSimulatorNew
DevRandomSimulator is the program, which simulates $cat /dev/random functionality. DevRandomSimulator program produces the [dev_random_replica] file at the location of your choice and constantly re-generating its content with new entropy data.

NOTE: Content of this file is being replaced with the entropy data coming from 3 different random algorithms: 1) Entropy data based upon System.nanoTime() seed 2) Entropy data based upon SecureRandom-related seed 3) Entropy data based upon UUID.randomUUID().getMostSignificantBits() seed

NOTE: results from all 3 entropy data sources are combined and re-shuffled.

Please use following commands to view produced results:

${FILE_DIR}/> cat dev_random_replica

or 
${FILE_DIR}/> cat dev_random_replica | base64

DevRandomSimulator 是模拟 $cat /dev/random 功能的程序。DevRandomSimulator 程序会在您选择的位置生成 [dev_random_replica] 文件，并不断使用新的熵数据重新生成其内容。

注意：此文件的内容正在替换为来自 3 种不同随机算法的熵数据：1) 基于 System.nanoTime() 种子的熵数据 2) 基于 SecureRandom 相关种子的熵数据 3) 基于 UUID 的熵数据。 randomUUID().getMostSignificantBits() 种子

注意：来自所有 3 个熵数据源的结果被合并并重新洗牌。

请使用以下命令查看生成的结果：

${FILE_DIR}/> cat dev_random_replica

或 ${FILE_DIR}/> cat dev_random_replica | base64
