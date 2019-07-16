---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5c5cbb57b66927d9b4246e3303bd3a76218be5e8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738038"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerActivityCounts(period='D7')')
    .get();

```