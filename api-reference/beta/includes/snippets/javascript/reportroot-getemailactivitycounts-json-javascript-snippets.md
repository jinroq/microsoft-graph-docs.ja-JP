---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 98927824ccb8196193d18ab307c1c6f06315d581
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527378"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailActivityCounts(period='D7')')
    .version('beta')
    .get();

```