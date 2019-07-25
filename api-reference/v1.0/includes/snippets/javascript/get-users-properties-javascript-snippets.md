---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 74d8efe099cf1a3d7f8fe5423a78577e1a7c5f68
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733760"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .select('displayName,givenName,postalCode')
    .get();

```