---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 64b7670e4d32322d0e486185cc8e840dc56462c0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/recent')
    .get();

```