---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 30d354ee47e4bc4cfcc9ef85d0a9837b16037e32
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/{domain-name}/serviceConfigurationRecords')
    .get();

```