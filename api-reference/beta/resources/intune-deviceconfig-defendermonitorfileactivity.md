---
title: defenderMonitorFileActivity 列挙型
description: ファイルアクティビティの監視に使用できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5c9c5bedbb07a89b51deb25942caeb5385f60e0a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333549"
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



