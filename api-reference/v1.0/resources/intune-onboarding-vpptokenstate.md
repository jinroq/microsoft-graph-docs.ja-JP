---
title: vppTokenState 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
author: tfitzmac
ms.openlocfilehash: e034f9712e2ef40b40b209935ed96f07b35cdbb9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321183"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|既定の状態。|
|有効です|1|トークンは、有効です。|
|有効期限が切れてください。|2|トークンの期限が切れています。|
|無効です|3|トークンが有効ではありません。|
|assignedToExternalMDM|4|トークンは、別の MDM サービスによって管理されます。|



