---
title: deviceManagementExchangeAccessStateReason 列挙型
description: デバイスの Exchange アクセス状態の理由。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ecd0e44a03a894ef21dfd35a97ac4f1bc272705
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942102"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスの Exchange アクセス状態の理由。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|Exchange から検出されたアクセス状態の理由はありません|
|不明|1-d|不明なアクセス状態の理由|
|exchangeGlobalRule|pbm-2|Exchange グローバルルールによって決定されるアクセス状態|
|Exchange個性 Alrule|1/3|Exchange の個々のルールによって決定されるアクセス状態|
|exchangeDeviceRule 方法|2/4|Exchange デバイスルールによって決定されるアクセス状態|
|exchangeUpgrade|5|Exchange アップグレードのためのアクセス状態|
|exchangeMailboxPolicy|シックス|Exchange メールボックスポリシーによって決定されるアクセス状態|
|も|7|Exchange によって決定されるアクセス状態|
|要件|8 |コンプライアンスの課題によって付与されるアクセス状態|
|notCompliant|9 |コンプライアンスの課題によるアクセス状態の取り消し|
|notEnrolled|10 |管理の課題によるアクセス状態の取り消し|
|unknownLocation|個|不明な場所のためのアクセス状態|
|mfaRequired|スリー|MFA チャレンジによるアクセス状態|
|azureADBlockDueToAccessPolicy|第|AAD アクセスポリシーによって無効にされたアクセス状態|
|compromisedPassword|約|侵害されたパスワードによって取り消されたアクセス状態|
|deviceNotKnownWithManagedApp|16|管理対象アプリケーションのチャレンジによって取り消されたアクセス状態|




