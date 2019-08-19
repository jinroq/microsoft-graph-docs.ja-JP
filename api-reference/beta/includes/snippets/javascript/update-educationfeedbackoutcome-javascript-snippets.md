---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e489cd204df061c71246b4b25252dd2bc15d0233
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationOutcome = {
    @odata.type:"#microsoft.graph.educationFeedbackOutcome",
    feedback:{
        text:{
            content:"This is feedback for the assignment as a whole.",
            contentType:"text"
        }
    }
};

let res = await client.api('/education/me/assignments/{id}/submissions/{id}/outcomes/{id}')
    .version('beta')
    .update({educationOutcome : educationOutcome});

```