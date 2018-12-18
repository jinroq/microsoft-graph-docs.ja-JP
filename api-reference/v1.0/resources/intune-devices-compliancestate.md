---
title: complianceState 列挙型
description: コンプライアンス状態です。
author: tfitzmac
ms.openlocfilehash: 3045685518f1c7718f9a5f46cd10e0add6fe05b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330276"
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



