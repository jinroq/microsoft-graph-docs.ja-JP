---
title: deviceManagementExchangeAccessStateReason 列挙型
description: デバイスの Exchange のアクセス状態の理由です。
ms.openlocfilehash: 691992262cf318a8fdc30573ea9bf5c0f0b29cf1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020892"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイスの Exchange のアクセス状態の理由です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|Exchange から検出アクセス状態の理由もなく|
|不明|1|不明なアクセスの状態の理由|
|exchangeGlobalRule|2|Exchange グローバル規則によって決定されるアクセスの状態|
|exchangeIndividualRule|3|Exchange の個別の規則によって決定されるアクセスの状態|
|exchangeDeviceRule|4|アクセス状態のデバイスの交換の規則によって決定されます。|
|exchangeUpgrade|5|Exchange のアップグレードのためのアクセスの状態|
|exchangeMailboxPolicy|6|Exchange メールボックス ポリシーで定義されたアクセスの状態|
|その他の|7|アクセス状態が Exchange によって決定されます。|
|準拠|8|コンプライアンスの課題によって与えられたアクセスの状態|
|notCompliant|9|コンプライアンスの課題によって失効アクセス状態|
|notEnrolled|10|アクセスの状態管理の課題によって失効|
|unknownLocation|12|不明な場所のためのアクセスの状態|
|mfaRequired|13|MFA の課題のためのアクセスの状態|
|azureADBlockDueToAccessPolicy|14|AAD アクセス ポリシーによって無効にするアクセスの状態|
|compromisedPassword|15|アクセス状態が危険にさらされたパスワードが無効|
|deviceNotKnownWithManagedApp|16|マネージ アプリケーションの課題によって失効アクセス状態|



