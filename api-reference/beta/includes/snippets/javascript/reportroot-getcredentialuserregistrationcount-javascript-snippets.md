---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5d8373da26a8b0d94b74eabb24e3287da3fcadff
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874115"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getCredentialUserRegistrationCount')
    .version('beta')
    .get();

```