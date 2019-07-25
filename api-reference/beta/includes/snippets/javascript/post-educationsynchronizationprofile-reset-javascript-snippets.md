---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 51bc86a97b9fc11e3e5dc14427d503abac3bdc68
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712474"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/reset')
    .version('beta')
    .post();

```