---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6eae99e66da1b1b0416a1f7772ae0886d74303ae
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476481"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}')
    .get();

```