---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8cd991dae06278d77a74bd69fd3de70678eef6dd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741154"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupSettingTemplates')
    .get();

```