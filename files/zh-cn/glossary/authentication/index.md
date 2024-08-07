---
title: 认证
slug: Glossary/Authentication
l10n:
  sourceCommit: 66afe9b59c609043c91e51487cfcecaecbbadb3d
---

{{GlossarySidebar}}

**认证**通常是证明某个事实是真实的过程。更具体地说，在 Web 安全中，它是验证某个实体（例如用户）所声称的身份的过程。这使得系统能够决定是否授予用户他们请求的访问权限，例如登录到特定帐户。

认证通常通过用户提供用户标识符以及{{glossary("credential", "凭据")}}（例如密码、一次性短信代码或使用私钥签名的断言）来执行。然后系统检查用户标识符和凭据之间的绑定，以便决定是否对用户进行认证。

认证信息，也称为*认证因素*，通常分为三类：

- 用户所知道的东西，例如密码。
- 用户所拥有的东西，例如手机。
- 用户自身的特征，例如指纹。

多因素认证（MFA）系统要求用户提供多于一个因素：例如，密码与发送到用户手机的一次性代码的组合。

## 参见

- {{rfc("4949", "互联网安全术语表")}}
