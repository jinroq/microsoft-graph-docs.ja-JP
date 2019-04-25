---
title: 自動 updatemode 列挙型
description: 自動更新モードで可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fd45ff85cbab934aa2549f13ee3e6671c65f9ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575178"
---
# <a name="automaticupdatemode-enum-type"></a>自動 updatemode 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

自動更新モードで可能な値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|notifydownload|1 |ダウンロードを通知します。|
|autoInstallAtMaintenanceTime|2 |メンテナンス時に自動インストールします。|
|autoInstallAndRebootAtMaintenanceTime|3 |メンテナンス時に自動的にインストールおよび再起動します。|
|autoInstallAndRebootAtScheduledTime|4 |スケジュールされた時刻に自動インストールおよび再起動します。|
|autoInstallAndRebootWithoutEndUserControl|5 |エンドユーザーコントロールを使用せずに自動インストールおよび再起動|



