---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b72c0d4ce215d90e1d524a0e95bd02374ab9c494
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437980"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')')
    .version('beta')
    .delete();

```