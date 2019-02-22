---
title: devicemanagementexchangeaccesslevel 列挙型
description: Exchange のアクセスレベル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc84149f9ca6b178807e4bd70984fe1abfff6a09
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174236"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a>devicemanagementexchangeaccesslevel 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Exchange のアクセスレベル。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|.0|Exchange でデバイスアクセスルールが構成されていません。|
|使う|1-d|デバイスへのアクセスを Exchange に許可します。|
|拒否|pbm-2|デバイスによる Exchange へのアクセスをブロックします。|
|済み|1/3|Exchange でデバイスを検疫します。|




