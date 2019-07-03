---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 93449caadbdbec00b4982d450771b3a2eb3db193
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485976"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/follow')
    .version('beta')
    .post();

```