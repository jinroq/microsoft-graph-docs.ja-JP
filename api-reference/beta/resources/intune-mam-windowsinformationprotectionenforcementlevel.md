---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: 仕掛品の保護の実施のレベルに指定できる値
author: tfitzmac
ms.openlocfilehash: cb30ffb58b129fc302d7896c148072a54b98c0a2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315163"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a>windowsInformationProtectionEnforcementLevel 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

仕掛品の保護の実施のレベルに指定できる値
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noProtection|0|なしの保護の実施|
|encryptAndAuditOnly|1|暗号化し、[監査のみ]|
|encryptAuditAndPrompt|2|暗号化、監査、およびメッセージを表示|
|encryptAuditAndBlock|3|暗号化、監査、およびブロック|





