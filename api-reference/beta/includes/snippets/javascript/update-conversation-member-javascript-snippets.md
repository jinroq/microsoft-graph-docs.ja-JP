---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 73a96ac91b80a9d508bab9c05087714c214b6960
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36634007"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
  roles: ["owner"]
};

let res = await client.api('/teams/{id}/channels/{id}/members/{id}')
    .version('beta')
    .update(conversationMember);

```