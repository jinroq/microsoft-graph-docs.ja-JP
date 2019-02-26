---
title: defendermonitorfileactivity 列挙型
description: ファイルアクティビティの監視に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d04d7a34de9c08c12d17c994381683c160bef1c4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152592"
---
# <a name="defendermonitorfileactivity-enum-type"></a>defendermonitorfileactivity 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ファイルアクティビティの監視に使用できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|無効にする|1-d|ファイルの監視処理を無効にします。|
|monitorallfiles|pbm-2|すべてのファイルを監視します。|
|monitorIncomingFilesOnly|1/3| 受信ファイルのみを監視します。|
|monitorOutgoingFilesOnly|2/4|送信ファイルのみを監視します。|




