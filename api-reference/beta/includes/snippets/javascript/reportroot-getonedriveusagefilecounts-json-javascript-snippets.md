---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2f89bbb2984203b197f4adc835dd3f3a0934f3a5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719149"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageFileCounts(period='D7')')
    .version('beta')
    .get();

```