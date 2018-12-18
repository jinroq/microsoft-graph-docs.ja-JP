---
title: teamSpecialization 列挙型
description: チームの特別なユース ケースをについて説明します。
author: nkramer
ms.openlocfilehash: 2e17f03374457ff8ddd9d3941eb56bebbec2dde6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348014"
---
# <a name="teamspecialization-enum-type"></a>teamSpecialization 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[チーム](../resources/team.md)が特定のユース ケースの目的として かどうかを示します。 各[チーム](../resources/team.md)の特殊化では、固有の動作とその使用例を対象としての経験へのアクセスを持ちます。 既定では 'なし' です。

## <a name="members"></a>メンバー

| メンバー             | 値 | 説明                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| none               | 0     | 既定の標準的なチームの経験を提供するチームのタイプです。          |
| unknownFutureValue | 7     | 列挙型の将来の拡張用のプレース ホルダーとして予約されている値を sentinel します。 |
