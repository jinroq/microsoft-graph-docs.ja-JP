---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションのコントロールの種類の使用可能な値
author: tfitzmac
ms.openlocfilehash: d53c2d0f7996edfab610e4206f4d2815ba4000b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310263"
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



