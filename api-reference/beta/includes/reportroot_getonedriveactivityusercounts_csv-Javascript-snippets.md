---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 87d4624772a43a14660e2777dbca66a78051b6db
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```