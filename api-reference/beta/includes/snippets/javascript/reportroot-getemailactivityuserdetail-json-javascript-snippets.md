---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d4f97c03391cbdacb9fc35057eb4065002516835
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527371"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailActivityUserDetail(period='D7')')
    .version('beta')
    .get();

```