---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 733dd832a0712ff3d7c9a48067cd65d283c2f961
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464609"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/checkout')
    .version('beta')
    .post();

```