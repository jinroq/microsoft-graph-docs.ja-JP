---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5b4f67ec6410a05378ae441b7b97eb88bfd24cfc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')')
    .version('beta')
    .get();

```