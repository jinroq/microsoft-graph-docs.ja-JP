---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 861b6a3f6d88f4d62ca54fcbbfc4afac9611c7ac
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageUserDetail(period='D7')')
    .get();

```