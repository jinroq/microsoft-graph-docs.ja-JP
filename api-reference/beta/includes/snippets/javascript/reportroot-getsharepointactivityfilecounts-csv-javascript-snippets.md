---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 20ccd274ee71c51404db0c8bb475b7a3ee0da45d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719111"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityFileCounts(period='D7')')
    .version('beta')
    .get();

```