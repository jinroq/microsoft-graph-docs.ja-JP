---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 358d859c524b38b7a37a4f604b9f40880b4bf498
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleSettings = {
    id: "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    elevationDuration: "PT8H",
    notificationToUserOnElevation: false,
    ticketingInfoOnElevation: true,
    mfaOnElevation: false,
    maxElavationDuration: "PT0S",
    minElevationDuration: "PT0S",
    lastGlobalAdmin: false,
    isMfaOnElevationConfigurable: true,
    approvalOnElevation: false,
    approverIds: ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
};

let res = await client.api('/privilegedRoles/{id}/settings')
    .version('beta')
    .put(privilegedRoleSettings);

```