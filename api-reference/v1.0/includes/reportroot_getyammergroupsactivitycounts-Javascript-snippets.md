---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 678214ebce17cfb1cbb4d3e218cc4d2fb7f2fe04
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468761"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerGroupsActivityCounts(period='D7')')
    .get();

```