---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ebfca6a4001f3be672ee174065d6395f59997c3f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739529"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActivationCounts')
    .get();

```