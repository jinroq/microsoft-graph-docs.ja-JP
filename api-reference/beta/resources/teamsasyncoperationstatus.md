---
title: teamsAsyncOperationStatus 列挙型
description: TeamsAsyncOperation の現在の状態について説明します。
ms.openlocfilehash: f553242ace983651b8d4fda77370de712f9d08b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067431"
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