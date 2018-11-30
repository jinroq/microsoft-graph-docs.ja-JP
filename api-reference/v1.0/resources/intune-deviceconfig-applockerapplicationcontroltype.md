---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションのコントロールの種類の使用可能な値
ms.openlocfilehash: 703cc18dfee49a01adb3cd4f61c5d7e99e30fb00
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020752"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 列挙型

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



