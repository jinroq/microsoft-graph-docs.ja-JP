---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 73106003169e48e9a41d91dd4dac54222e35bee0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/permissions')
    .version('beta')
    .get();

```