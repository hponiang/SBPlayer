# SBPlayer

##### 使用方法：拖拽SBPlayer文件到项目中，导入SBPlayer.h (如果已开启沙盒，需勾选Client，并在info.plist文件中添加ATS)

```

@interface ViewController()<SBPlayerDelegate>

@property (nonatomic,strong) SBPlayer *player;

@end
@implementation ViewController

- (void)viewDidLoad {
    [super viewDidLoad];

    self.player = [[SBPlayer alloc]initWithURL:[NSURL URLWithString:@"http://download.3g.joy.cn/video/236/60236937/1451280942752_hd.mp4"] view:self.view withDelegate:self ];

}
```
