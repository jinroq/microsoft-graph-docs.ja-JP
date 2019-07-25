---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0789a1b03208a0b5505b19a1ecb0a842192a689f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858939"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members/{id}/$ref')
    .version('beta')
    .delete();

```