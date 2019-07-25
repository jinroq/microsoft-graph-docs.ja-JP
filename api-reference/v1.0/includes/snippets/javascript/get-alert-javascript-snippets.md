---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0ba7c1161064bbdea7e895322b40cb063ad26aeb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733425"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/alerts/{alert_id}')
    .get();

```