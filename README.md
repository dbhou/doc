php框架汇总
 
	安装PHP依赖管理工具composer
		curl -sS https://getcomposer.org/installer | php
		mv composer.phar /usr/local/bin/composer
		
	配置composer使用国内节点镜像
		composer config -g repo.packagist composer https://packagist.phpcomposer.com （全局配置，推荐配置）
		composer config repo.packagist composer https://packagist.phpcomposer.com （修改当前项目的配置，必须保证项目下必须有相应的composer.json）
		
	安装thinkphp并创建项目
		composer create-project topthink/think test.think.com dev-master --prefer-dist
		离线包：http://down.thinkphp.cn/download.php?key=MTQ2NjY3MTYyMY+xf56Yl8jWw3hrysCosKuvonSttJyTqLTMZt6yY9nZgaGsnIS4x5O6m52XtLaOaryliZ20nJhnx7t3zrF1rJOZf6Gol5em0MR3apOyzHubxaWAr7Kh06HJpn/Yrp+o2pt/raOPlqqRwohr176lcqu7a4WhynaUq8qrgNG+iZLMkIlycA
		demo：https://github.com/Hifone/Hifone
	
	安装laravel并创建项目
		composer create-project laravel/laravel test.laravel.com --prefer-dist
		离线包：http://down.golaravel.com/laravel/laravel-v5.2.15.zip
	
	安装symfony并创建项目
		composer create-project symfony/framework-standard-edition test.symfony.com
		使用symfony自带工具
			curl -LsS https://symfony.com/installer -o /usr/local/bin/symfony
			symfony new test.symfony.com (2.8|3.1.x|lts 分支号)
		离线包：
			
	安装Yii并创建项目
		composer global require "fxp/composer-asset-plugin:~1.1.1" 安装 Composer asset plugin，它是通过 Composer 管理 bower 和 npm 包所必须的，此命令全局生效，一劳永逸。
		composer create-project yiisoft/yii2-app-basic test.yii.com
