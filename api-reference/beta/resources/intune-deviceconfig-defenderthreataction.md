---
title: defenderThreatAction 列挙型
description: Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d092d5a23fc006a9accdf9062a27cd79f323d208
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400271"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|0|更新プログラム定義に基づいたアクションを適用します。|
|クリーン|1|検出された脅威をクリーニングします。|
|検査|2|検出された脅威を隔離します。|
|remove|3|検出された脅威を削除します。|
|許可します。|4|脅威の検出を許可します。|
|ユーザー定義|5|検出された脅威に対して実行するアクションを決定するユーザーを許可します。|
|ブロック|6|検出された脅威をブロックします。|




