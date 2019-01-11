---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザー アカウントに使用できる値は、設定を制御します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 02ea15b10b0eb6a789456d9f91e63ca3249a0933
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810662"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a>windowsUserAccountControlSettings 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows ユーザー アカウントに使用できる値は、設定を制御します。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|ユーザー定義、既定値、ない目的。|
|alwaysNotify|1|常に次のように通知します。|
|notifyOnAppChanges|2|アプリケーションの変更を通知します。|
|notifyOnAppChangesWithoutDimming|3|デスクトップを暗転しないアプリケーションの変更を通知します。|
|neverNotify|4|通知しません。|



