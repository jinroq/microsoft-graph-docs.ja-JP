---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションコントロールタイプの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b1e463959cf4b5b39076fcf200b1c61ea0e73c0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257079"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 列挙型

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



