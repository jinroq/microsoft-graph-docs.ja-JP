---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0bd7b6b87cfeac5424e4ae130df6433a105a226c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513220"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices')
    .get();

```