---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f9a3a1f6423a29dfcafe0969eb7785c78d310620
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738991"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/children')
    .get();

```