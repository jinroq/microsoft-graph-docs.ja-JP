---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4522a0023aa71d878bcf30c38626898dd5216d50
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718948"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```