---
title: 自動 updatemode 列挙型
description: 自動更新モードで可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9af00bda442c1a152820323fc0b7e1ddfcd8c384
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791482"
---
# <a name="automaticupdatemode-enum-type"></a>自動 updatemode 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

自動更新モードで可能な値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|notifydownload|1-d|ダウンロードを通知します。|
|autoInstallAtMaintenanceTime|pbm-2|メンテナンス時に自動インストールします。|
|autoInstallAndRebootAtMaintenanceTime|1/3|メンテナンス時に自動的にインストールおよび再起動します。|
|autoInstallAndRebootAtScheduledTime|2/4|スケジュールされた時刻に自動インストールおよび再起動します。|
|autoInstallAndRebootWithoutEndUserControl|5|エンドユーザーコントロールを使用せずに自動インストールおよび再起動|
|windowsdefault|シックス|Windows の既定値にリセットします。|





