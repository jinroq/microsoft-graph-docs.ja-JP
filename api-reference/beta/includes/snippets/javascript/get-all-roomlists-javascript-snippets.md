---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f2e2188321e1337d1f4098e44de62dd35de86f89
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/places/microsoft.graph.roomlist')
    .version('beta')
    .get();

```