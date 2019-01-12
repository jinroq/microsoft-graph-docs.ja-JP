---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型
description: キラーの資格情報の設定で使用できる値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d284b81632c5ba48fa4c658719203a74fdf52837
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952742"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

キラーの資格情報の設定で使用できる値です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|UEFI ロックせずに以前設定されている場合リモート資格情報の保護をオフにします。|
|enableWithUEFILock|1|UEFI ロックで資格情報の保護をオンにします。|
|enableWithoutUEFILock|2|UEFI ロックせず資格情報の保護をオンにします。|





