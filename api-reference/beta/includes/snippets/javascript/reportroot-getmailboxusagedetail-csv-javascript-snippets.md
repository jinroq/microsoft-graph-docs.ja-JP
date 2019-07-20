---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2dd336e96f309110a8a1aae4eb7a5b58035b30d7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageDetail(period='D7')')
    .version('beta')
    .get();

```