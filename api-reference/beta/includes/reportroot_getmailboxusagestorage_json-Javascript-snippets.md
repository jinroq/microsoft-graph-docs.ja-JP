---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6849ded5a40453ad62b3d34bd53fbd9ef97c1469
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441914"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageStorage(period='D7')')
    .version('beta')
    .get();

```