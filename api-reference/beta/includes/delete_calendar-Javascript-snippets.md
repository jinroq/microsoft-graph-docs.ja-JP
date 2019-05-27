---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f1e8864c7df9977afb77d2e22dcc9a88eb755684
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438806"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar')
    .version('beta')
    .delete();

```