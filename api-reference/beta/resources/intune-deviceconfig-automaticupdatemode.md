---
title: automaticUpdateMode 列挙型
description: 自動更新モードを使用可能な値です。
ms.openlocfilehash: b7eac8337d6c8286e538bbe98b5ecbc13a448628
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072253"
---
# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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





