---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b12f9562b06c3b6abd27fd511188603bed634215
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462016"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReview = {
    displayName:"TestReview new name"
};

let res = await client.api('/accessReviews/006111db-0810-4494-a6df-904d368bd81b')
    .version('beta')
    .update({accessReview : accessReview});

```