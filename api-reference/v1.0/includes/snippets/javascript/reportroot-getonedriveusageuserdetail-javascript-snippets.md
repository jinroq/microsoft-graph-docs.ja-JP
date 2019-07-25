---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4985b651dfcc755b1b26b77d81d731fc288e8897
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733256"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageAccountDetail(period='D7')')
    .get();

```