---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9d49f28d4d6958147ebec1d92ad00b1583fa3131
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464130"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```