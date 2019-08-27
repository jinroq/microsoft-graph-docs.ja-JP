---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 95457d909b072d145d41265551fae0e3e423cf86
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637922"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const participant = {
  clientContext: "d45324c1-fcb5-430a-902c-f20af696537c",
  participantMixerLevels: [
    {
      participant: "550fae72-d251-43ec-868c-373732c2704f",
      exclusive: true,
      ducking: {
        rampActive: 50,
        rampInactive: 50,
        lowerLevel: 10,
        upperLevel: 50
      },
      sourceLevels: [
        {
          participant: "632899f8-2ea1-4604-8413-27bd2892079f",
          level: 50,
          duckOthers: false
        }
      ]
    }
  ]
};

let res = await client.api('/app/calls/{id}/participants/configureMixer')
    .version('beta')
    .post(participant);

```