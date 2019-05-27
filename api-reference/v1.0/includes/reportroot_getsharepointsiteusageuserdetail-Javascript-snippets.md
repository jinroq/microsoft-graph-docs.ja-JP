---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5c7952c9af82743ea730b06cb3df7f9f31c7de58
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477006"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsageDetail(period='D7')')
    .get();

```