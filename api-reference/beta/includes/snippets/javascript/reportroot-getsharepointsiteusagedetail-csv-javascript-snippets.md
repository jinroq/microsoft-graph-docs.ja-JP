---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7df26e0895bc5f326c5ca7c2cbc27aaec68148d9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719025"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsageDetail(period='D7')')
    .version('beta')
    .get();

```