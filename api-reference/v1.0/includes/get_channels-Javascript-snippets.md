---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9837f3f644031111acdbd735dfc4ad9111f0584
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456776"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels')
    .get();

```