---
title: win32LobAppRegistryDetectionType 列挙型
description: サポートされているすべてのレジストリデータ検出の種類が含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c19d2dfa0c19be1d61178c25fdd04615d2f9dbd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534424"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a>win32LobAppRegistryDetectionType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

サポートされているすべてのレジストリデータ検出の種類が含まれます。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|.0|構成されていません。|
|ある|1 |指定されたレジストリキーまたは値が存在します。|
|doesNotExist|2 |指定したレジストリキーまたは値が存在しません。|
|string|3 |文字列型 (String) の値を指定します。|
|整数|4 |整数型 (Integer) の値です。|
|バージョン|5 |バージョン値の種類。|





