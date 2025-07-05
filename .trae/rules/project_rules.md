# 项目 Git 协作规则（当前项目：xxx 仓库）  
## 1. 仓库与分支约束  
- 远程仓库默认关联：`https://github.com/你的用户名/项目名`（推送前自动校验远程地址 ）。  
- 分支命名强制规范：  
  - 功能分支：`feature/需求名`（如 `feature/login-verify` ）；  
  - 修复分支：`fix/问题描述`（如 `fix/login-crash` ）。  

## 2. 提交与 PR 流程  
- 提交信息必须包含 **关联 Issue**（如 `fix: 修复登录页空白 #123` ，#123 是 Issue 编号 ）。  
- 创建 PR 时，自动调用 GitHub MCP 生成模板：  
  ```markdown  
  ## 变更内容  
  - 修复登录页验证码不显示问题（关联 #123 ）  
  - 新增单元测试：src/login.test.js  

  ## 测试情况  
  - 本地测试通过：验证码显示正常，登录流程无报错  # Temporary line for PR
