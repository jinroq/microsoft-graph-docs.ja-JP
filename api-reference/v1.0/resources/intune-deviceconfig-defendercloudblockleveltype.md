---
title: defenderCloudBlockLevelType 列挙型
description: クラウド ・ ブロック ・ レベルで使用できる値
author: tfitzmac
ms.openlocfilehash: 19c101cc82673009a39d6545f7340fabf65b287a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326615"
---
# <a name="defendercloudblockleveltype-enum-type"></a>defenderCloudBlockLevelType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

クラウド ・ ブロック ・ レベルで使用できる値
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|既定値、レベルおよび検出のリスクを増大させることがなく強固な検出は、既定の Windows Defender のウイルス対策プログラムのブロック機能を使用して正規のファイル|
|高|1|高には、強力な検出レベルが適用されます。|
|highPlus|2|高 + 高レベルを使用し、追加の保護手段を適用します。|
|zeroTolerance|3|耐は、すべての不明な実行可能ファイルをブロックします。|



