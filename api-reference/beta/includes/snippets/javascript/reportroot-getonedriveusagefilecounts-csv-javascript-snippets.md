---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2f89bbb2984203b197f4adc835dd3f3a0934f3a5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504134"
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