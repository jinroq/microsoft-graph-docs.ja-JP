---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 00c1580c9d377bc2ceef004f8e4dfea47bce94f3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727656"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageUserCounts(period='D7')')
    .version('beta')
    .get();

```