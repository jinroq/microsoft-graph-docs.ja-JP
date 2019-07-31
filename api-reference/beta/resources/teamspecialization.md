---
title: teamSpecialization 列挙型
description: チームの特別なユースケースについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: enumPageType
ms.openlocfilehash: a0ff737b196cc486aa01d5e0f5a34c30edc7c8bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964428"
---
# <a name="teamspecialization-enum-type"></a>teamSpecialization 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](../resources/team.md)が特定のユースケースを対象としているかどうかを示します。 各[チーム](../resources/team.md)の特殊化は、そのユースケースを対象とした固有の動作とエクスペリエンスにアクセスできます。 既定値は ' none ' です。

## <a name="members"></a>メンバー

| メンバー             | 値 | 説明                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| none               | .0     | 標準のチーム環境を提供するチームの既定の種類。          |
| educationStandard  | 1-d     | 教育機関ユーザーによって作成されたチーム。 教育機関のユーザーによって作成されたすべてのチームの種類は Edu です。 |
| educationClass     | pbm-2     | クラスに対して最適化されたチームの作業環境。 これにより、O365 間での機能のセグメンテーションが可能になります。 |
| educationProfessionalLearningCommunity | 1/3 | PLC 用に最適化されたチームの作業環境。 [この記事](https://en.wikipedia.org/wiki/Professional_learning_community)の「PLC」を参照してください。 |
| educationStaff     | 2/4     |  チームの種類は、組織内のスタッフ (プリンシパルなど) が管理者であり、教師が管理者であり、専門のノートブックを備えたチームのメンバーである場合に最適な環境を提供します。 詳細については、「[教育機関向け OneNote スタッフノートブック](https://www.onenote.com/staffnotebookedu)」を参照してください。 |
| Unknownfuturevalue という | 7     | 列挙型を今後拡張するためのプレースホルダーとして予約されている Sentinel 値。 |
