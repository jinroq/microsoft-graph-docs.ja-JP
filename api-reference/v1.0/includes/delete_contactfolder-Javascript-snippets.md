---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ba3fe481771a2456bac05866560cee5317b0285c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}')
    .delete();

```