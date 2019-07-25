---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: adf8d6d56b9132a5cf4872ac5b171210b2e67696
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860458"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/users')
    .version('beta')
    .get();

```