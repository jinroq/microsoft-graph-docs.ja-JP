---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3eb9024bc3b355fb4f48f4418bd79a2f6042a68f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739153"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/delta?token=latest')
    .get();

```