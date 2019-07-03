---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0f01b00ad0cf5fea70ef358f3527efd90f597130
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527090"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')')
    .version('beta')
    .get();

```