---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 54ba0d5865ed42cc38d01d75e3b695a6f71ce0af
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440857"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageStorage(period='D7')')
    .version('beta')
    .get();

```