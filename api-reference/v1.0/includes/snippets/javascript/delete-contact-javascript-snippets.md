---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e5bbf1ea0f9af75e5f03a539150f6608e81b6f8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741089"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contacts/{id}')
    .delete();

```