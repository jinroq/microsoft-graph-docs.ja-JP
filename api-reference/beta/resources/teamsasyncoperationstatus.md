---
title: teamsAsyncOperationStatus 列挙型
description: teamsAsyncOperation の現在の状態を表します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bd44b7e1feabfba75edaa9bbeb88f1f0ed7a00f0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345748"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>teamsAsyncOperationStatus 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[teamsAsyncOperation](teamsasyncoperation.md)の現在の状態を表します。

## <a name="members"></a>メンバー

| メンバー | 値| 説明 |
|:---------------|:--------|:----------|
|無効です|.0|無効な値です。|
|notStarted|1-d|操作は開始されていません。|
|inProgress|pbm-2|操作が実行されています。|
|失敗|1/3|操作が正常に完了しました。|
|フェール|2/4|操作は失敗しました。|
