---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ec12617f91b4022c416cd7edb484c8408e55d2eb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715811"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/sites')
    .get();

```