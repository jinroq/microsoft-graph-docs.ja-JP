---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dfb983ccf82d4a8c171f7e960e90b950cd2a56e2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731065"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageStorage(period='D7')')
    .get();

```