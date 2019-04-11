---
title: devicemanagementexchangeaccesslevel 列挙型
description: Exchange のアクセスレベル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c235d31e97b570f70145884349eaef6e2254194c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802465"
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





