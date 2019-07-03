---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: aa5b6050018a44a65f06f1bb85b8997963e5691e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526988"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/uploadUrl')
    .version('beta')
    .get();

```