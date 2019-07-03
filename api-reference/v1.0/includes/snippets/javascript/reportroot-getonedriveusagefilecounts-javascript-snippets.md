---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7f3ab46d2e8fc2d0bc7333d46cabeeef70578b15
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513196"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageFileCounts(period='D7')')
    .get();

```