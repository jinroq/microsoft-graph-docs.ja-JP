---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: fead773494ff3eaebca6d22d65a1622128d63c42
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719917"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .version('beta')
    .skiptoken('c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA=')
    .get();

```