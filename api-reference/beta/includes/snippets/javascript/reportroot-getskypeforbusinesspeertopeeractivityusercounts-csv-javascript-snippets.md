---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dbb5aa9929e5e8fd1cabdc35434b297c0e3e0141
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726649"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```