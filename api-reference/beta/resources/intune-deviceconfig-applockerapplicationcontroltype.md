---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションのコントロールの種類の使用可能な値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3bc89620a6dd13a65cfe40f37ba2f775e6a9c83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425723"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>appLockerApplicationControlType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

AppLocker アプリケーションのコントロールの種類の使用可能な値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|デバイス デフォルト値が選択されていないアプリケーションのコントロールの種類です。|
|enforceComponentsAndStoreApps|1|Windows コンポーネント、ストア アプリケーションを強制します。|
|auditComponentsAndStoreApps|2|Windows コンポーネント、ストア アプリケーションを監査します。|
|enforceComponentsStoreAppsAndSmartlocker|3|Windows コンポーネント、アプリケーションとスマート ロッカーを格納します。|
|auditComponentsStoreAppsAndSmartlocker|4|Windows コンポーネントを監査し、アプリケーションとスマート ロッカーを格納します。|




