---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションコントロールタイプの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22d108dd3bad90341031d1e965948a9daa59efa1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141357"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

AppLocker アプリケーションコントロールタイプの可能な値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|デバイスの既定値。アプリケーションコントロールの種類は選択されていません。|
|enforceComponentsAndStoreApps|1-d|Windows コンポーネントおよびストアアプリを適用します。|
|auditComponentsAndStoreApps|pbm-2|Windows コンポーネントおよびストアアプリを監査します。|
|enforceComponentsStoreAppsAndSmartlocker|1/3|Windows コンポーネント、ストアアプリ、およびスマートロッカーを適用します。|
|auditComponentsStoreAppsAndSmartlocker|2/4|Windows コンポーネント、ストアアプリ、およびスマートロッカーを監査します。|




