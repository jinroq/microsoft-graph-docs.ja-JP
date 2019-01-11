---
title: teamSpecialization 列挙型
description: チームの特別なユース ケースをについて説明します。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 18e1993272a94df989066cf95d01b6a4f66fd8d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826041"
---
# <a name="teamspecialization-enum-type"></a>teamSpecialization 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[チーム](../resources/team.md)が特定のユース ケースの目的として かどうかを示します。 各[チーム](../resources/team.md)の特殊化では、固有の動作とその使用例を対象としての経験へのアクセスを持ちます。 既定では 'なし' です。

## <a name="members"></a>メンバー

| メンバー             | 値 | 説明                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| none               | 0     | 既定の標準的なチームの経験を提供するチームのタイプです。          |
| unknownFutureValue | 7     | 列挙型の将来の拡張用のプレース ホルダーとして予約されている値を sentinel します。 |
