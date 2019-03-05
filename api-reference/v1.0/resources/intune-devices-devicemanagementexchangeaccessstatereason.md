---
title: deviceManagementExchangeAccessStateReason 列挙型
description: デバイスの Exchange アクセス状態の理由。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c014afbf22c58f89f8b8926058e28a5ca2d1a1d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252036"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスの Exchange アクセス状態の理由。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|Exchange から検出されたアクセス状態の理由はありません|
|不明|1-d|不明なアクセス状態の理由|
|exchangeglobalrule|pbm-2|Exchange グローバルルールによって決定されるアクセス状態|
|exchange個性 alrule|1/3|Exchange の個々のルールによって決定されるアクセス状態|
|exchangedevicerule 方法|2/4|Exchange デバイスルールによって決定されるアクセス状態|
|exchangeupgrade|5|Exchange アップグレードのためのアクセス状態|
|exchangeMailboxPolicy|シックス|Exchange メールボックスポリシーによって決定されるアクセス状態|
|も|7|Exchange によって決定されるアクセス状態|
|要件|~|コンプライアンスの課題によって付与されるアクセス状態|
|notcompliant|i-9|コンプライアンスの課題によるアクセス状態の取り消し|
|notenrolled|個|管理の課題によるアクセス状態の取り消し|
|unknownLocation|個|不明な場所のためのアクセス状態|
|mfarequired|スリー|MFA チャレンジによるアクセス状態|
|azureADBlockDueToAccessPolicy|第|AAD アクセスポリシーによって無効にされたアクセス状態|
|compromisedPassword|約|侵害されたパスワードによって取り消されたアクセス状態|
|devicenotknownwithmanagedapp|16|管理対象アプリケーションのチャレンジによって取り消されたアクセス状態|



