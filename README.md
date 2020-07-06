# water_blue_grub

## 安装

1. 把此文件夹改名为`water_blue_grub`放入`/boot/grub/themes`

2. ubuntu: 在`/etc/default/grub`增加或修改

```
GRUB_GFXMODE="1024x768"
GRUB_THEME="/boot/grub/themes/water_blue_grub/theme.txt"
GRUB_BACKGROUND="/boot/grub/themes/water_blue_grub/background.png"
```

deepin: 在`/etc/grub.d/00_header`第二行增加

```
GRUB_GFXMODE="1024x768"
GRUB_THEME="/boot/grub/themes/water_blue_grub/theme.txt"
```

在`/etc/grub.d/05_debian_theme`第二行增加

```
GRUB_BACKGROUND="/boot/grub/themes/water_blue_grub/background.png"
```

3. 运行`sudo update-grub`

## 配置

```
sudo apt install grub-customizer
```

使用`grub-customizer`修改菜单名称为短名称,比如Ubuntu,Deepin这样的.

修改排序,把高级选项下移到底部.

默认显示3个菜单,需要4个的,修改`/boot/grub/themes/water_blue_grub/theme.txt`中的 `boot_menu` -> `height = 264`为350
