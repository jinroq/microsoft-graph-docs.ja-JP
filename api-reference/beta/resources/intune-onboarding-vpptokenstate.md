---
title: vppTokenState 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8e2148cccbb891b1c139abd9d15ba424b3b3e9b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967379"
---
# <a name="vpptokenstate-enum-type"></a>vppTokenState 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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





