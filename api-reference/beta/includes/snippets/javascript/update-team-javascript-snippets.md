---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e69480937211fa8afc0289f9e98ce345834bf32b
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  memberSettings: {
    allowCreateUpdateChannels: true
  },
  messagingSettings: {
    allowUserEditMessages: true,
    allowUserDeleteMessages: true
  },
  funSettings: {
    allowGiphy: true,
    giphyContentRating: "strict"
  },
  discoverySettings: {
    showInTeamsSearchAndSuggestions: true
  }
};

let res = await client.api('/teams/{id}')
    .version('beta')
    .update(team);

```