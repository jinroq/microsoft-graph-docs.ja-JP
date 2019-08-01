---
title: 自動 Updatemode 列挙型
description: 自動更新モードで可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3a0cc2d3918573fca6480c6eecd07889534cda4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028575"
---
# <a name="automaticupdatemode-enum-type"></a>自動 Updatemode 列挙型

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



