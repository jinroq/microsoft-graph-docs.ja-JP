---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: acf2af8d025c2f2ada9b6e1ecdff3a3e82e819d9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736476"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive')
    .get();

```