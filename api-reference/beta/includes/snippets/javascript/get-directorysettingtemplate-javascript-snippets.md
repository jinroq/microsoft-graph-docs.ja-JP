---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e9aca11225022e41f7a26803b263796583eff6db
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directorySettingTemplates/{id}')
    .version('beta')
    .get();

```