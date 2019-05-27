---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4e33dc08cd4de82c57a6534a781df43e0ee06789
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463940"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```