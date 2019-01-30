---
title: teamSpecialization 列挙型
description: チームの特別なユース ケースをについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c89f3ef993e55e28f5558f99c3ef87ad5174bc65
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640323"
---
# <a name="teamspecialization-enum-type"></a>teamSpecialization 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](../resources/team.md)が特定のユース ケースの目的として かどうかを示します。 各[チーム](../resources/team.md)の特殊化では、固有の動作とその使用例を対象としての経験へのアクセスを持ちます。 既定では 'なし' です。

## <a name="members"></a>メンバー

| メンバー             | 値 | 説明                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| none               | 0     | 既定の標準的なチームの経験を提供するチームのタイプです。          |
| educationStandard  | 1     | 教育ユーザーによって作成されたチームです。 教育ユーザーによって作成されたすべてのチームは、Edu の種類です。 |
| educationClass     | 2     | クラス用に最適化されたチームの経験。 O365 全体の機能の区分の基準が使用できます。 |
| educationProfessionalLearningCommunity | 3 | チームの経験を PLC 用に最適化されました。 PLC の詳細については[ここで](https://en.wikipedia.org/wiki/Professional_learning_community)。 |
| educationStaff     | 4     |  管理者、教師、プリンシパルと同様に、スタッフのリーダーは、場所、組織内のスタッフの作業を最適化するためのチーム タイプは、専用のノートブックに付属しているチームのメンバーです。 詳細については、[教育のスタッフ ノートを OneNote](https://www.onenote.com/staffnotebookedu)を参照してください。 |
| unknownFutureValue | 7     | 列挙型の将来の拡張用のプレース ホルダーとして予約されている値を sentinel します。 |
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/resources/teamspecialization.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
