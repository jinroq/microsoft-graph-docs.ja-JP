---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange のアクセスの状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f66f8372b5bd087ad620fa86d8e0beff8b3eb3a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401069"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a>deviceManagementExchangeAccessState 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスの Exchange のアクセスの状態です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|none|0|Exchange から検出アクセス状態がないです。|
|不明|1|Exchange へのデバイスのアクセス状態は不明です。|
|許可|2|デバイスが Exchange へのアクセス権を持つ|
|ブロック|3|デバイスが Exchange でブロックされています。|
|検疫|4|デバイスが Exchange の検疫します。|




