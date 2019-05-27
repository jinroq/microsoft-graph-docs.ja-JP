---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 268d52a604c904c8970f3fa9bcfafe7fc5bbf051
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478798"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/revokeSignInSessions')
    .version('beta')
    .post();

```