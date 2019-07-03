---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9f8547294388b0d3d8ff141e1da2fc6cf9a9d2c2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageUserDetail(period='D7')')
    .version('beta')
    .get();

```