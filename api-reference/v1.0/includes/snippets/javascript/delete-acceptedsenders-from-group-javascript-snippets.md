---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: da46308b57793f95b054578120553ffca1250a6e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856520"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/acceptedSenders/$ref')
    .delete();

```