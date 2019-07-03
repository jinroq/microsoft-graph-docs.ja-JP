---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 51d2e0f672602f670cbbe735753753221ecd85ad
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504307"
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