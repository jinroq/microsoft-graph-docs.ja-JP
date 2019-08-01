---
title: deviceRegistrationState 列挙型
description: デバイス登録の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 933ea7cf16421ecadd9bb23b4594d8ca0f5e767b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030731"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 列挙型

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス登録の状態。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notRegistered 済み|.0|デバイスが登録されていません。|
|い|pbm-2|デバイスは登録されています。|
|破棄|1/3|デバイスがブロックされているか、ワイプされているか、破棄されています。|
|keyConflict|2/4|デバイスにキーの競合があります。|
|approvalPending|5|デバイスの承認が保留中です。|
|certificateReset|シックス|デバイス証明書がリセットされました。|
|notRegisteredPendingEnrollment|7|デバイスは登録されておらず、登録が保留されていません。|
|不明|8 |デバイス登録の状態が不明です。|



