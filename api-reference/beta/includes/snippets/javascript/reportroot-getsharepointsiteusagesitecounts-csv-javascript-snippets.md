---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 12e6fc9eafa76f4c5230d40f0a6ab3d296c46a43
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726981"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsageSiteCounts(period='D7')')
    .version('beta')
    .get();

```