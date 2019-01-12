---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザー アカウントに使用できる値は、設定を制御します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0475d8fb013cbb07f8d69a659f8ecde2eb580e43
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972475"
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



