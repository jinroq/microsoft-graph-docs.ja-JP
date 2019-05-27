---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bd0fcd02bf174e1058ae5be8f40f81dcef4a2191
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474213"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/agreements/'id'')
    .version('beta')
    .expand('files')
    .get();

```