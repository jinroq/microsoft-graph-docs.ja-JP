---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7d7859e6b7cb2ad8456234a2e4f565a752f4d544
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop')
    .version('beta')
    .post();

```