---
title: deviceManagementExchangeAccessStateReason 列挙型
description: デバイスの Exchange のアクセス状態の理由です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 956eca76c4ccabe0d3d5c003d38e35ced172febf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917413"
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



