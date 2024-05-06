## 表情制作

### 在线gif制作工具

https://ezgif.com/

https://lvgl.io/tools/imageconverter

### 注意事项

1、动图帧数控制、大小控制

2、RAM占用粗略计算

帧数 * width * high + LV_deepth（颜色深度）

例如  10 * 320 * 240  + LV_deepth(忽略) = 约 750KB RAM占用

### 说明

如果觉得本视频对你有帮助，可以点一个免费的赞吗，谢谢大家！

![](.\Emoji\静态\close_eys_slow.GIF)

### Example

```c
LV_IMG_DECLARE(close_eys_slow);
lv_obj_t *img;

void main()
{
    img = lv_gif_create(lv_scr_act());
    lv_gif_set_src(img, &close_eys_slow);
    
    .....
}
```

