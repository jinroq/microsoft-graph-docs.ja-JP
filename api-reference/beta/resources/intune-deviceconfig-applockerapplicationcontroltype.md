---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションのコントロールの種類の使用可能な値
author: tfitzmac
ms.openlocfilehash: 0d6190170d6f6695a3303047f9ccb193afd248f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330206"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

AppLocker アプリケーションのコントロールの種類の使用可能な値
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|デバイス デフォルト値が選択されていないアプリケーションのコントロールの種類です。|
|enforceComponentsAndStoreApps|1|Windows コンポーネント、ストア アプリケーションを強制します。|
|auditComponentsAndStoreApps|2|Windows コンポーネント、ストア アプリケーションを監査します。|
|enforceComponentsStoreAppsAndSmartlocker|3|Windows コンポーネント、アプリケーションとスマート ロッカーを格納します。|
|auditComponentsStoreAppsAndSmartlocker|4|Windows コンポーネントを監査し、アプリケーションとスマート ロッカーを格納します。|





