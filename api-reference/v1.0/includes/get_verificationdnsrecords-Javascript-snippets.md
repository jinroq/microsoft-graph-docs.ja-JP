---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e601b6df65be2ea410f94015b417ff916e0db5df
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478301"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/{domain-name}/verificationDnsRecords')
    .get();

```