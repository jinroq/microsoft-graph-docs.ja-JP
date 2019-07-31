---
title: teamsAsyncOperationStatus 列挙型
description: TeamsAsyncOperation の現在の状態を表します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 35975d122adf6411afc6fe4c382d1ff46b41e263
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007684"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>teamsAsyncOperationStatus 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[TeamsAsyncOperation](teamsasyncoperation.md)の現在の状態を表します。

## <a name="members"></a>メンバー

| メンバー | 値| 説明 |
|:---------------|:--------|:----------|
|無効です|.0|無効な値です。|
|notStarted|1-d|操作は開始されていません。|
|inProgress|pbm-2|操作が実行されています。|
|失敗|1/3|操作が正常に完了しました。|
|フェール|2/4|操作は失敗しました。|
