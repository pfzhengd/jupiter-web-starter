## AI 客服 README

## CDN 地址
```JS
https://cdn.miaa.top/jarvis/v0/loader.js
```

## 引用示例

```JS

Jarvis.define(function(){
  const im = new JarvisIM()
  im.mount('#root') // #root 为要挂载 IM 聊天窗体的工具
  im.show({
    serviceName:"VOLA", // 客服的名称 (必填)
    userId:"SIB800",    // 当前用户的ID （可选)
  })
})

```

## Jarvis 可选参数
```JS
export interface IJarvisOptions {
  // 用户ID
  userId?: string
  // 应用编码
  appCode?: string
  // 设备信息
  deviceInfoId?: string
  // 客服名称
  serviceName: string
  // 用户类型
  userType?: string
  // 商业编码（用于区分市场）
  bizCode?:'cd935848c2'|undefined
  // IM 主色  (与渐变色一起使用)
  mainColor?:string
  // IM 渐变色（与主色一起使用）
  fadeMainColor?:string
}
```