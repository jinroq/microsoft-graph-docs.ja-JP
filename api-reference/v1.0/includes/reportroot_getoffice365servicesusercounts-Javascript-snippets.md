---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a3c60644f70f39ef46386e695e00fe8dffee81b8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478693"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ServicesUserCounts(period='D7')')
    .get();

```