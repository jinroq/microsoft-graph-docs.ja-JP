---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c958607343b85bfbecb889fdbad4cdada78c3fda
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735798"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageAccountCounts(period='D7')')
    .get();

```