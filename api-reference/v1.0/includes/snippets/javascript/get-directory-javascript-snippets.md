---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e8fb8e9f5008aa54b23a567b9b294b7cbea2c42f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513217"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/deletedItems/{object-id}')
    .get();

```