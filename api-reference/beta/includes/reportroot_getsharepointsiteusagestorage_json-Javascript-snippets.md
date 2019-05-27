---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fbaca6101a75ab8a75ef4f9a308443c37f5d5220
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464637"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsageStorage(period='D7')')
    .version('beta')
    .get();

```