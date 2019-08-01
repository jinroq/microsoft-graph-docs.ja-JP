---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションコントロールタイプの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9b4a20a79454f1aba1f162812a7fc4d7a324c359
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028568"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 列挙型

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

AppLocker アプリケーションコントロールタイプの可能な値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|デバイスの既定値。アプリケーションコントロールの種類は選択されていません。|
|enforceComponentsAndStoreApps|1-d|Windows コンポーネントおよびストアアプリを適用します。|
|auditComponentsAndStoreApps|pbm-2|Windows コンポーネントおよびストアアプリを監査します。|
|enforceComponentsStoreAppsAndSmartlocker|1/3|Windows コンポーネント、ストアアプリ、およびスマートロッカーを適用します。|
|auditComponentsStoreAppsAndSmartlocker|2/4|Windows コンポーネント、ストアアプリ、およびスマートロッカーを監査します。|



