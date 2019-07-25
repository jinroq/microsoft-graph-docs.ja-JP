---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 14f2a6b1f720b25874e16fe65fde307d959cd0ac
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718900"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsagePages(period='D7')')
    .version('beta')
    .get();

```