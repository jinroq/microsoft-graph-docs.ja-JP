---
title: teamspecialization 列挙型
description: チームの特別なユースケースについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c89f3ef993e55e28f5558f99c3ef87ad5174bc65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553653"
---
# <a name="teamspecialization-enum-type"></a>teamspecialization 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](../resources/team.md)が特定のユースケースを対象としているかどうかを示します。 各[チーム](../resources/team.md)の特殊化は、そのユースケースを対象とした固有の動作とエクスペリエンスにアクセスできます。 既定値は ' none ' です。

## <a name="members"></a>メンバー

| メンバー             | 値 | 説明                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| なし               | .0     | 標準のチーム環境を提供するチームの既定の種類。          |
| educationStandard  | 1      | 教育機関ユーザーによって作成されたチーム。 教育機関のユーザーによって作成されたすべてのチームの種類は Edu です。 |
| educationClass     | 2      | クラスに対して最適化されたチームの作業環境。 これにより、O365 間での機能のセグメンテーションが可能になります。 |
| educationProfessionalLearningCommunity | 3  | PLC 用に最適化されたチームの作業環境。 [この記事](https://en.wikipedia.org/wiki/Professional_learning_community)の「PLC」を参照してください。 |
| educationStaff     | 4      |  チームの種類は、組織内のスタッフ (プリンシパルなど) が管理者であり、教師が管理者であり、専門のノートブックを備えたチームのメンバーである場合に最適な環境を提供します。 詳細については、「[教育機関向け OneNote スタッフノートブック](https://www.onenote.com/staffnotebookedu)」を参照してください。 |
| unknownfuturevalue という | 7      | 列挙型を今後拡張するためのプレースホルダーとして予約されている Sentinel 値。 |
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/resources/teamspecialization.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
