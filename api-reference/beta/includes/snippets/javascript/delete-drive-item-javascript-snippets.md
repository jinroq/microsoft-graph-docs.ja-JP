---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fae9fd3c81ae147a3c565b1d9795a1b2ba94803a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861263"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}')
    .version('beta')
    .delete();

```