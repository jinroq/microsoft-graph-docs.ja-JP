---
title: teamsAsyncOperationStatus 列挙型
description: TeamsAsyncOperation の現在の状態について説明します。
author: nkramer
ms.openlocfilehash: 49b5b81999714627b1a1acd42df208594123b262
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332005"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>teamsAsyncOperationStatus 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

の[teamsAsyncOperation](teamsasyncoperation.md)の現在の状態について説明します。

## <a name="members"></a>メンバー

| メンバー | 値| 説明 |
|:---------------|:--------|:----------|
|無効です|0|値が無効です。|
|未開始|1|操作は開始されていません。|
|inProgress|2|操作が行われています。|
|成功しました|3|操作が正常に完了しました。|
|失敗しました。|4|処理に失敗しました。|