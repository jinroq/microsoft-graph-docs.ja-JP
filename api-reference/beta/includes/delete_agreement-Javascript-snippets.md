---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 54ff0424a9e21f11827bf9ed278e02370291b96c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439065"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/agreements/'id'')
    .version('beta')
    .delete();

```