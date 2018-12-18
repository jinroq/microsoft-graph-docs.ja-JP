---
title: automaticUpdateMode 列挙型
description: 自動更新モードを使用可能な値です。
author: tfitzmac
ms.openlocfilehash: d1bf3903b71dbd06be9151d67a925f374eb1f803
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344045"
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





