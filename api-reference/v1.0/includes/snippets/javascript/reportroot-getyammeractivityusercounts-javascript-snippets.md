---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 06d21f70029b324439afab18bf90c3e7d242dc0e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738017"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerActivityUserCounts(period='D7')')
    .get();

```