---
title: complianceState 列挙型
description: コンプライアンス状態です。
ms.openlocfilehash: 041a2267b952d37e0aeef29e1325e5cb7b561ed7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023659"
---
# <a name="compliancestate-enum-type"></a>complianceState 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

コンプライアンス状態です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|不明。|
|準拠|1|準拠していません。|
|準拠していません。|2|デバイスは非準拠、企業のリソースがブロックされました。|
|競合|3|その他の規則と競合しています。|
|エラー|4|エラー。|
|inGracePeriod|254|デバイスは非準拠ですが、社内リソースへのアクセスにはまだ|
|configManager|255|構成マネージャーによって管理されます。|



