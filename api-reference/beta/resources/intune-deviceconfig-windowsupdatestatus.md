---
title: windowsUpdateStatus 列挙型
description: ビジネス構成デバイスの状態に関する Windows update
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ace0b42b09093ce2e9d485271ec607ffd618c9e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978690"
---
# <a name="windowsupdatestatus-enum-type"></a>windowsUpdateStatus 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ビジネス構成デバイスの状態に関する Windows update

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|upToDate|.0|保留中の更新はありません。保留中の再起動更新プログラムはありません。更新は失敗しています。|
|pendingInstallation|1-d|承認されていない更新プログラムが含まれている保留中の更新プログラムがあります。 保留中の再起動更新はありません。更新は失敗しません。|
|pendingReboot|pbm-2|再起動が必要な更新プログラムがあります。 失敗した更新はありません。|
|フェール|1/3|デバイスにインストールできなかった更新プログラムがあります。|





