---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1a7a9fd8404184ee96bf74c469bd7f7519978589
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/delta')
    .version('beta')
    .header('Prefer','return=minimal')
    .select('displayName,description,mailNickname')
    .get();

```