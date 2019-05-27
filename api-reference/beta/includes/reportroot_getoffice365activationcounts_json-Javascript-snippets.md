---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7147fd71f9a33c55f910e3f446d279f860db06a9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441802"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActivationCounts')
    .version('beta')
    .get();

```