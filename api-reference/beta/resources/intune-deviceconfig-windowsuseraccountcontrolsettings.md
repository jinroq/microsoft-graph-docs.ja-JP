---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザー アカウントに使用できる値は、設定を制御します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ff348fd33e6bbc8370378783cf0a517a205ea101
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399816"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a>windowsUserAccountControlSettings 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows ユーザー アカウントに使用できる値は、設定を制御します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|ユーザー定義、既定値、ない目的。|
|alwaysNotify|1|常に次のように通知します。|
|notifyOnAppChanges|2|アプリケーションの変更を通知します。|
|notifyOnAppChangesWithoutDimming|3|デスクトップを暗転しないアプリケーションの変更を通知します。|
|neverNotify|4|通知しません。|




