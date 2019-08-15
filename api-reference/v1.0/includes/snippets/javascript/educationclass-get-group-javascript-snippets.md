---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2b5b122bffe443161071d1beafb8dfa94b281047
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}/group')
    .get();

```