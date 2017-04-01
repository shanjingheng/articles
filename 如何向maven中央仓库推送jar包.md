##流程简介：
在[https://issues.sonatype.org](https://issues.sonatype.org/)注册帐号

create一个issue，填写信息为pom文件描述

等待管理审核后会在issue下comment给出发布仓库的地址

上传自己gpg加密的公钥到maven服务器``gpg --keyserver hkp://pool.sks-keyservers.n
et --send-keys XXX``

需要上传的文件需要有8个.xxx.pom,xxx-jar,xxx-javadoc,xxx-sources以及经过gpg加密的4个.asc文件

pom文件格式需要规范，没有问题的情况下，可以点击release

第一次发布需要在回到issue下进行一次comment告诉管理员已经发布了release版本，请求同步到中央仓库