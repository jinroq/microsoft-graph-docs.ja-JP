---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションコントロールタイプの可能な値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1b3e5ec545f4466eb080f20839e12c7e5972cc0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981581"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

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





