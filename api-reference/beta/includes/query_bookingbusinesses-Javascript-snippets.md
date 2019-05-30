---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0ac1d65b7ab257bbfadfcf772dfd0ee0bf653194
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses?query=Adventure')
    .version('beta')
    .get();

```