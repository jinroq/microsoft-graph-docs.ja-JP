---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a43575cee0bf173082f1e67664df9e3dfa43d2e8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736213"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{siteId}/drives')
    .get();

```