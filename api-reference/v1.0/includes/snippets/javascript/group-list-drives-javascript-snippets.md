---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f8a20e9595a24006fa5c006e4ede9cc966219f08
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496102"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{groupId}/drives')
    .get();

```