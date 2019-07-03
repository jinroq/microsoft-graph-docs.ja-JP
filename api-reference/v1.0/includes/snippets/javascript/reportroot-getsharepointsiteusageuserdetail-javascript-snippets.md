---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5c7952c9af82743ea730b06cb3df7f9f31c7de58
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495729"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsageDetail(period='D7')')
    .get();

```