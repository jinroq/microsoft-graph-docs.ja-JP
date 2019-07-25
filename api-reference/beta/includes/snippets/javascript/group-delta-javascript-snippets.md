---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5ee9271eb6a5410c0dbba0d0c0f017070be7e06e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/delta')
    .version('beta')
    .get();

```