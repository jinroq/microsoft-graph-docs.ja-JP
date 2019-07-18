---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 51d2e0f672602f670cbbe735753753221ecd85ad
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707593"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}/messages/{id}')
    .version('beta')
    .get();

```