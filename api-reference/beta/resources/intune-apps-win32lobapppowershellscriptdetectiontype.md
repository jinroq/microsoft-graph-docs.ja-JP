---
title: win32LobAppPowerShellScriptDetectionType 列挙型
description: サポートされているすべての Powershell スクリプトの出力検出の種類が含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4dc45a3b7ec8fe2732a89022fd3c74c0959bbc1c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809397"
---
# <a name="win32lobapppowershellscriptdetectiontype-enum-type"></a>win32LobAppPowerShellScriptDetectionType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

サポートされているすべての Powershell スクリプトの出力検出の種類が含まれます。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|構成されていません。|
|string|1-d|出力データの種類は文字列です。|
|dateTime|pbm-2|出力データの種類は、日付/時刻です。|
|整数|1/3|出力データの種類は整数です。|
|浮動小数点数|2/4|出力データの種類は float です。|
|バージョン|5|出力データの種類はバージョンです。|
|ブール値|シックス|Output データ型はブール値です。|





