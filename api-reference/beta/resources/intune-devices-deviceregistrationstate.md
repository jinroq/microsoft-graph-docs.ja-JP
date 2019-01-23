---
title: deviceRegistrationState 列挙型
description: デバイス登録のステータス。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90f2dc7f8c11940fa01047d8c61f23c8f0389ed8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396757"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス登録のステータス。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notRegistered|0|デバイスは登録されていません。|
|登録|2|デバイスが登録されています。|
|失効|3|デバイスがブロックされている、消去した廃止します。|
|keyConflict|4|デバイスには、キーの競合があります。|
|approvalPending|5|デバイスは、承認が保留中です。|
|certificateReset|6|デバイスの証明書をリセットするとします。|
|notRegisteredPendingEnrollment|7|デバイスが登録されていないと登録を保留中です。|
|不明|8|デバイス ライセンス登録のステータスは不明です。|




