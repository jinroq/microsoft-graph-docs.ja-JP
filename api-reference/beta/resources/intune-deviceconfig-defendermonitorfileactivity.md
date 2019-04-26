---
title: defendermonitorfileactivity 列挙型
description: ファイルアクティビティの監視に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2888484f90bb3389fa7b7b12c79ce386d1bfd2db
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563505"
---
# <a name="defendermonitorfileactivity-enum-type"></a>defendermonitorfileactivity 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ファイルアクティビティの監視に使用できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|無効にする|1 |ファイルの監視処理を無効にします。|
|monitorallfiles|2 |すべてのファイルを監視します。|
|monitorIncomingFilesOnly|3 | 受信ファイルのみを監視します。|
|monitorOutgoingFilesOnly|4 |送信ファイルのみを監視します。|





