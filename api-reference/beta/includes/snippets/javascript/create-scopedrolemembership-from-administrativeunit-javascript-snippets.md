---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fafa220d2bcc66c3d6befe041a383ffb4513da45
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637858"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const scopedRoleMembership = {
  roleId: "roleId-value",
  roleMemberInfo: {
    id: "id-value"
  }
};

let res = await client.api('/administrativeUnits/{id}/scopedRoleMembers')
    .version('beta')
    .post(scopedRoleMembership);

```