---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f4b3dae19d10a1e68287fc07fef0e4ce09477afa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710904"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder')
    .version('beta')
    .post();

```