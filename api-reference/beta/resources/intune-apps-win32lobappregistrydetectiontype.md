---
title: win32LobAppRegistryDetectionType 列挙型
description: サポートされているすべてのレジストリデータ検出の種類が含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 62028eefbfa85bceb669cbe8cc4bee8261d5837e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158458"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a>win32LobAppRegistryDetectionType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

サポートされているすべてのレジストリデータ検出の種類が含まれます。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|構成されていません。|
|ある|1-d|指定されたレジストリキーまたは値が存在します。|
|doesNotExist|pbm-2|指定したレジストリキーまたは値が存在しません。|
|string|1/3|文字列型 (String) の値を指定します。|
|integer|2/4|整数型 (Integer) の値です。|
|version|5|バージョン値の種類。|




