---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 53e711ba87e75573e4e32226473b617a5b8889fd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719443"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActivationsUserDetail')
    .version('beta')
    .get();

```