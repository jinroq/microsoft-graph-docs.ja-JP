---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションコントロールタイプの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b1e463959cf4b5b39076fcf200b1c61ea0e73c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575129"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

AppLocker アプリケーションコントロールタイプの可能な値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|デバイスの既定値。アプリケーションコントロールの種類は選択されていません。|
|enforceComponentsAndStoreApps|1 |Windows コンポーネントおよびストアアプリを適用します。|
|auditComponentsAndStoreApps|2 |Windows コンポーネントおよびストアアプリを監査します。|
|enforceComponentsStoreAppsAndSmartlocker|3 |Windows コンポーネント、ストアアプリ、およびスマートロッカーを適用します。|
|auditComponentsStoreAppsAndSmartlocker|4 |Windows コンポーネント、ストアアプリ、およびスマートロッカーを監査します。|



