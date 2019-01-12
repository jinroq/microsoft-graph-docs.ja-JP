---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションのコントロールの種類の使用可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 258a98b9ec4945c807a6aae2b34a178628952ac4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937958"
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



