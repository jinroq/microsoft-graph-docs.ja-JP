---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 98927824ccb8196193d18ab307c1c6f06315d581
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727729"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailActivityCounts(period='D7')')
    .version('beta')
    .get();

```