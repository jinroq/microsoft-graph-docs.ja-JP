---
title: automaticUpdateMode 列挙型
description: 自動更新モードを使用可能な値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d982c4c9ee524712c212eba1b8b44349d0a70377
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402637"
---
# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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
|windowsDefault|6|Windows の既定値にリセットされます。|




