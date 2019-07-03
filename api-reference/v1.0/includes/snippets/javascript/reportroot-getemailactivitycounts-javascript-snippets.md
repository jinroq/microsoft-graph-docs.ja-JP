---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4785fc0d11825b0311d4a34cfabdd495b1d509b6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailActivityCounts(period='D7')')
    .get();

```