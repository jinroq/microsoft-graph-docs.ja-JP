---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f54c219214ad96e17a770962cbe8f04983394e24
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .version('beta')
    .get();

```