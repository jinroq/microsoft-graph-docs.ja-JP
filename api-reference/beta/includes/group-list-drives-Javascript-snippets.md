---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3dc9982fe65c71aaa336cd8596736a70691b55a0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444875"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{groupId}/drives')
    .version('beta')
    .get();

```