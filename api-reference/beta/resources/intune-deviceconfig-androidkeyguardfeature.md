---
title: Androidkeygu/Feature 列挙型
description: Android keyguard 機能。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f62e2a8055dd6e8f46ac40a06d0c8f0bfc7677ad
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988939"
---
# <a name="androidkeyguardfeature-enum-type"></a>Androidkeygu/Feature 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android keyguard 機能。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|未構成。この値は無視されます。|
|デジタル|1-d|セキュリティで保護された keyguard 画面でのカメラの使用状況。|
|受け取る|pbm-2|セキュリティで保護された keyguard 画面での通知の表示。|
|未 Redacted通知|1/3|Secure keyguard 画面での unredacted 通知の表示。|
|trustAgents|2/4|Secure keyguard 画面の場合にエージェントの状態を信頼します。|
|デジタル|5|セキュリティで保護された keyguard 画面の場合の指紋センサーの使用量。|
|remoteInput|シックス|セキュリティで保護された keyguard 画面での通知テキスト入力。|
|allFeatures|7|セキュリティで保護された keyguard 画面上のすべての keyguard 機能。|





