---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e21f3c8beebf41c8365d31ae54cf209005fd8e0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416438"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group')
    .version('beta')
    .get();

```