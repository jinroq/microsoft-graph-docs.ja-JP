---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f2a76e6b52174fd503c3d0917f4b1915095bf176
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/sort')
    .get();

```