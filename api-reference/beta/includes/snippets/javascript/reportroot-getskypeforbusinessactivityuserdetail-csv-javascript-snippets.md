---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ce99740ccabce8c45740c1a9f663e384e0bca310
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527554"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessActivityUserDetail(period='D7')')
    .version('beta')
    .get();

```