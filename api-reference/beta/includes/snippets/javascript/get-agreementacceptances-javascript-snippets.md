---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: abaae7631defb1fb4d1526be6f09ada2cdb61cb2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527101"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/agreementAcceptances')
    .version('beta')
    .get();

```