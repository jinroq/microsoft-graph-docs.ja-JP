---
title: win32LobAppRegistryDetectionType 列挙型
description: すべて含まれているレジストリ データの検出の種類をサポートします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 188f206e42b55e0c2cc2f8b6ed831f19a4b2052a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411086"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a>win32LobAppRegistryDetectionType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

すべて含まれているレジストリ データの検出の種類をサポートします。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|構成されていません。|
|存在します。|1|指定したレジストリ キーまたは値が存在します。|
|doesNotExist|2|指定したレジストリ キーまたは値が存在しません。|
|string|3|値型の文字列を指定します。|
|integer|4|整数値型。|
|version|5|バージョンの値の型。|




