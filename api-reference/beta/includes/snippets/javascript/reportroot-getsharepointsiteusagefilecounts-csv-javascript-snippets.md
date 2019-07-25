---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d93f4ff260f410491874283213989f257734c84d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727027"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsageFileCounts(period='D7')')
    .version('beta')
    .get();

```