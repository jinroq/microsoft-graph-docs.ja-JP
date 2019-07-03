---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 055ad830aec3f7245be098bc8f2715a4c3ffd2a2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496067"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/createReplyAll')
    .post();

```