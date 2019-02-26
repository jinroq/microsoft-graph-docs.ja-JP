---
title: windowsUpdateType 列挙型
description: 更新プログラムを受信するブランチデバイス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f91657cabec59cf1307253d707ba632bf4f99463
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260222"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

更新プログラムを受信するブランチデバイス

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザーがを設定できるようにします。|
|all|1-d|半期チャネル (対象指定)。 デバイスは、半期チャネル (対象指定) から、適用可能なすべての機能の更新を取得します。|
|businessReadyOnly|pbm-2|半期チャネル デバイスは、半期チャネルから機能の更新を取得します。|
|windowsinsiderbuildfast|1/3|Windows Insider ビルド-Fast|
|windowsInsiderBuildSlow|2/4|Windows Insider ビルド-低速|
|windowsinsiderbuildrelease|5|Windows Insider ビルドをリリースする|



