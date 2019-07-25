---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3d0272d2eaa235e42145199d9b8030a24189dbcf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730709"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion')
    .post();

```