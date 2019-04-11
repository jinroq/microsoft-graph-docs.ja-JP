---
title: windowsUpdateType 列挙型
description: 更新プログラムを受信するブランチデバイス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 228cc5ba4b50681bfe78a15ef214d6f3ab2ebb17
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779693"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

更新プログラムを受信するブランチデバイス

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザーがを設定できるようにします。|
|すべての|1-d|半期チャネル (対象指定)。 デバイスは、半期チャネル (対象指定) から、適用可能なすべての機能の更新を取得します。|
|businessReadyOnly|pbm-2|半期チャネル デバイスは、半期チャネルから機能の更新を取得します。|
|windowsinsiderbuildfast|1/3|Windows Insider ビルド-Fast|
|windowsInsiderBuildSlow|2/4|Windows Insider ビルド-低速|
|windowsinsiderbuildrelease|5|Windows Insider ビルドをリリースする|





