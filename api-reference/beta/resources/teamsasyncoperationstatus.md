---
title: teamsAsyncOperationStatus 列挙型
description: TeamsAsyncOperation の現在の状態について説明します。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: b6af5c7218a6a9d8c0c5338beb8cdf9944a56c2e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858976"
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
