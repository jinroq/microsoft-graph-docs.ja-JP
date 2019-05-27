---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8daf93612223aaee9cc0e26c1c6b5a660924f588
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437469"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}')
    .version('beta')
    .delete();

```