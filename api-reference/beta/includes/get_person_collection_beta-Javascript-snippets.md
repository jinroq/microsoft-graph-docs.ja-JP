---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a82aca3ed7ea3a424def1b86d09da02c916d96c6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447895"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/people')
    .version('beta')
    .get();

```