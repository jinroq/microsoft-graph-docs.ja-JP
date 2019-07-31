---
title: defenderMonitorFileActivity 列挙型
description: ファイルアクティビティの監視に使用できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2039ca95b69f61b88e5b12b28b55977cb63c1b50
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001783"
---
# <a name="defendermonitorfileactivity-enum-type"></a>defenderMonitorFileActivity 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ファイルアクティビティの監視に使用できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|無効にする|1-d|ファイルの監視処理を無効にします。|
|monitorAllFiles|pbm-2|すべてのファイルを監視します。|
|monitorIncomingFilesOnly|1/3| 受信ファイルのみを監視します。|
|monitorOutgoingFilesOnly|2/4|送信ファイルのみを監視します。|





