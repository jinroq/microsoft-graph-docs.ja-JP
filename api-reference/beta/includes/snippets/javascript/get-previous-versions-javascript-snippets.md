---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: db6b92ff1baf16be8989c526fb75b4652dd67cfc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712859"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/versions')
    .version('beta')
    .get();

```