---
title: 自動 Updatemode 列挙型
description: 自動更新モードで可能な値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d2fffa3e1b1a5e7efa43d7ce653792247e3ad790
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983632"
---
# <a name="automaticupdatemode-enum-type"></a>自動 Updatemode 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

自動更新モードで可能な値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|notifyDownload|1-d|ダウンロードを通知します。|
|autoInstallAtMaintenanceTime|pbm-2|メンテナンス時に自動インストールします。|
|autoInstallAndRebootAtMaintenanceTime|1/3|メンテナンス時に自動的にインストールおよび再起動します。|
|autoInstallAndRebootAtScheduledTime|2/4|スケジュールされた時刻に自動インストールおよび再起動します。|
|autoInstallAndRebootWithoutEndUserControl|5|エンドユーザーコントロールを使用せずに自動インストールおよび再起動|
|windowsDefault|シックス|Windows の既定値にリセットします。|





