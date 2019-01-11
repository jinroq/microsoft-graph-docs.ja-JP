---
title: complianceState 列挙型
description: コンプライアンス状態です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53b17f258f577e0842dbfc81c6341303f6b43799
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820343"
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



