---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b32a87d85c4b35651c175ed06713221d1a3bc972
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485436"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/securityActions')
    .version('beta')
    .get();

```