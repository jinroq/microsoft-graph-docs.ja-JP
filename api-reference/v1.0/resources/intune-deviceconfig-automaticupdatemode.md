---
title: automaticUpdateMode 列挙型
description: 自動更新モードを使用可能な値です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07a6b410289ea6455d0f6756efa7d1ec4d735ce4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849988"
---
# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

自動更新モードを使用可能な値です。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|ユーザー定義|0|ユーザー定義、既定値、ない目的。|
|notifyDownload|1|ダウンロード時に通知します。|
|autoInstallAtMaintenanceTime|2|メンテナンス時に自動インストールします。|
|autoInstallAndRebootAtMaintenanceTime|3|自動インストールおよびメンテナンス時に再起動します。|
|autoInstallAndRebootAtScheduledTime|4|自動インストールし、スケジュールされた時刻に再起動します。|
|autoInstallAndRebootWithoutEndUserControl|5|自動インストールし、エンドユーザーの制御に再起動します|



