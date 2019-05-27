---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a92bd01e38dedce8f95e93459b18272152b9f064
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)')
    .get();

```