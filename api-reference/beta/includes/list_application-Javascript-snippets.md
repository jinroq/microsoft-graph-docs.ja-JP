---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6e9fd5aad905bc79ef588a57ab75e20b2a4ee10b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444329"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications')
    .version('beta')
    .get();

```