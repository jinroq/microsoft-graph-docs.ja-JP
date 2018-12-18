---
title: eapFastConfiguration 列挙型
description: EAP-FAST 構成の使用可能な設定です。
author: tfitzmac
ms.openlocfilehash: ba84adb86e9910df47bd236fd2bd348cbc9c8e6f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326363"
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





