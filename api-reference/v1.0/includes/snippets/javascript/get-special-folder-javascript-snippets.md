---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 961abf87d514e6716d1e34c0127231b3e7fb48cd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/special/{name}')
    .get();

```