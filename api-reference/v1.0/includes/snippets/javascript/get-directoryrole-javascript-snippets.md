---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b0a005b3623b82538daa5872e9e0b443dd8784a1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739101"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/{id}')
    .get();

```