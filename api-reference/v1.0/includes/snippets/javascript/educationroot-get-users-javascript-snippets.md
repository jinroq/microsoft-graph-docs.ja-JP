---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 86f7acda9ec44d8d1bfbd56ce8e97ae717450fe6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881434"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/users')
    .get();

```