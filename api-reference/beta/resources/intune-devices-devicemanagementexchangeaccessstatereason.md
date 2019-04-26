---
title: deviceManagementExchangeAccessStateReason 列挙型
description: デバイスの Exchange アクセス状態の理由。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dab2b0b39290568331a16473fd6eaf7286ce5df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570048"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスの Exchange アクセス状態の理由。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|なし|.0|Exchange から検出されたアクセス状態の理由はありません|
|不明|1 |不明なアクセス状態の理由|
|exchangeglobalrule|2 |Exchange グローバルルールによって決定されるアクセス状態|
|exchange個性 alrule|3 |Exchange の個々のルールによって決定されるアクセス状態|
|exchangedevicerule 方法|4 |Exchange デバイスルールによって決定されるアクセス状態|
|exchangeupgrade|5 |Exchange アップグレードのためのアクセス状態|
|exchangeMailboxPolicy|6 |Exchange メールボックスポリシーによって決定されるアクセス状態|
|も|7 |Exchange によって決定されるアクセス状態|
|要件|8 |コンプライアンスの課題によって付与されるアクセス状態|
|notcompliant|9 |コンプライアンスの課題によるアクセス状態の取り消し|
|notenrolled|10  |管理の課題によるアクセス状態の取り消し|
|unknownLocation|12 |不明な場所のためのアクセス状態|
|mfarequired|13 |MFA チャレンジによるアクセス状態|
|azureADBlockDueToAccessPolicy|14 |AAD アクセスポリシーによって無効にされたアクセス状態|
|compromisedPassword|15 |侵害されたパスワードによって取り消されたアクセス状態|
|devicenotknownwithmanagedapp|16 |管理対象アプリケーションのチャレンジによって取り消されたアクセス状態|





