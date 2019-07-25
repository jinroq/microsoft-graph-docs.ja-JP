---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2759a65cba2c5917bf42262886c0a50d7c89f47c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733998"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/secureScores')
    .top(1)
    .get();

```