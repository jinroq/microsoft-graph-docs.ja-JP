---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9d49f28d4d6958147ebec1d92ad00b1583fa3131
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```