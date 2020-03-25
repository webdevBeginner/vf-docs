# 接口

引擎创建后，可获取的相关周期函数以及可调用API

## 周期函数

### 日志与错误时的回调
onError(evt: IEvent): void;

### 初始化完成
onInit(): void;

### 数据初始化完成（资源加载完成）
onReady(): void;

### 场景创建完成
onSceneCreate(): void;

### 消息
onMessage(msg: IEvent): void;

### 卸载时触发
onDispose(): void;

## API

### 播放（播放地址|播放数据|恢复播放）
play(src?: any): void;

### 卸载
dispose(boolean?: boolean): void;

### 暂停
pause(): void;

### 恢复
resume(): void;

### 重置
reset(): void;

### 发送消息
message(msg: IEvent): void;

### 切换下一个场景
switchToNextScene(transition?: ITransitionData): void;

### 切换上一个场景
switchToPrevScene(transition?: ITransitionData): void;

### 切换特定场景
switchToSceneId(sceneId: string, transition?: ITransitionData): void;