---
title: deviceManagementExchangeAccessStateReason 列挙型
description: デバイスの Exchange のアクセス状態の理由です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7a076239e49c59cb95cd1c1f644bc9a2f1f906e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395861"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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




