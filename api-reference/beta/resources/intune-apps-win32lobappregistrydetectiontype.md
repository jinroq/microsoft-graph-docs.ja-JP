---
title: win32LobAppRegistryDetectionType 列挙型
description: サポートされているすべてのレジストリデータ検出の種類が含まれます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63f058d9b8b63c2177e597e39c655a0999f63595
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949648"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a>win32LobAppRegistryDetectionType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

サポートされているすべてのレジストリデータ検出の種類が含まれます。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|構成されていません。|
|ある|1-d|指定されたレジストリキーまたは値が存在します。|
|doesNotExist|pbm-2|指定したレジストリキーまたは値が存在しません。|
|string|1/3|文字列型 (String) の値を指定します。|
|整数|2/4|整数型 (Integer) の値です。|
|バージョン|5|バージョン値の種類。|




