---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1cb926d71b9c928f05f2e8f74739d441d8c886cb
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36846109"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/57dab8b1-894c-409a-b240-bd8beae78896')
    .version('beta')
    .delete();

```