---
title: 自動 Updatemode 列挙型
description: 自動更新モードで可能な値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e8d64f3af656a03bd02ecba5db2fbdab288f3693
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333885"
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



