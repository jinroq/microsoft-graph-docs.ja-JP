---
title: defenderCloudBlockLevelType 列挙型
description: クラウド ・ ブロック ・ レベルで使用できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b309184623cff19e44ee5afea311d46fa89210fb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425912"
---
# <a name="defendercloudblockleveltype-enum-type"></a>defenderCloudBlockLevelType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

クラウド ・ ブロック ・ レベルで使用できる値

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|既定値、レベルおよび検出のリスクを増大させることがなく強固な検出は、既定の Windows Defender のウイルス対策プログラムのブロック機能を使用して正規のファイル|
|高|1|高には、強力な検出レベルが適用されます。|
|highPlus|2|高 + 高レベルを使用し、追加の保護手段を適用します。|
|zeroTolerance|3|耐は、すべての不明な実行可能ファイルをブロックします。|




