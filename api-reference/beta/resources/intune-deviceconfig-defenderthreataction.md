---
title: defenderThreatAction 列挙型
description: 検出されたマルウェアの脅威を処理する Defender の既定のアクション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 57b5ecf73548bf67bcb1fbfb75ed0730cb308424
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333416"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

検出されたマルウェアの脅威を処理する Defender の既定のアクション。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|deviceDefault|.0|更新定義に基づいてアクションを適用します。|
|汚れ|1-d|検出された脅威を除去します。|
|済み|pbm-2|検出された脅威を検疫します。|
|remove|1/3|検出された脅威を削除します。|
|使う|2/4|検出された脅威を許可します。|
|自分のもの|5|検出された脅威に対して実行するアクションをユーザーが決定できるようにします。|
|拒否|シックス|検出された脅威をブロックします。|



