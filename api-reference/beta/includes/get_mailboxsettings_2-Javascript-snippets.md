---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 737ab32ec43dd4d84cf37c978bfed82b0afd39ef
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailboxSettings/automaticRepliesSetting')
    .version('beta')
    .get();

```