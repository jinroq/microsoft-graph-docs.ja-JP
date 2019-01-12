---
title: eapFastConfiguration 列挙型
description: EAP-FAST 構成の使用可能な設定です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65165929d388ed57f2651a0d277996e56d2f046e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954457"
---
# <a name="eapfastconfiguration-enum-type"></a>eapFastConfiguration 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

EAP-FAST 構成の使用可能な設定です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noProtectedAccessCredential|0|EAP-FAST クリデンシャル (PAC) の保護されたアクセスなしを使用します。|
|useProtectedAccessCredential|1|保護されたアクセス クリデンシャル (PAC) をを利用します。|
|useProtectedAccessCredentialAndProvision|2|使用してアクセスを保護するクリデンシャル (PAC) と PAC. を提供します。|
|useProtectedAccessCredentialAndProvisionAnonymously|3|保護されたアクセスの資格情報 (PAC)、PAC のプロビジョニングを使用して実行し、匿名で。|





