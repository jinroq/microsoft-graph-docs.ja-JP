---
title: リソースの種類のリスク
description: レベルのリスク、リスクの状態を集約して、リスクの詳細、リスクの高いユーザーのサインイン、または、イベントのリスクです。
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 48fda9624e45072240bc694b8b5e152fe3ef0764
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524822"
---
# <a name="risk-resource-type"></a>リソースの種類のリスク

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

レベルのリスク、リスクの状態を集約して、リスクの詳細、リスクの高いユーザーのサインイン、または、イベントのリスクです。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|`stateDetail`|riskDetail|危険なユーザー、サインインまたはリスク事象の特定の状態の背後にある '理由' を提供します。 可能な値: `none`、 `adminGeneratedTemporaryPassword`、 `userPerformedSecuredPasswordChange`、 `userPerformedSecuredPasswordReset`、 `adminConfirmedSigninSafe`、 `aiConfirmedSigninSafe`、 `userPassedMFADrivenByRiskBasedPolicy`、 `adminDismissedAllRiskForUser`、 `adminConfirmedSigninCompromised`、 `unknownFutureValue`。 値`none`アクションが実行されたことなしに、ユーザーまたはのサインインでこれまでにすることを意味します。 |
|`riskLevelAggregated`|riskLevel|危険なユーザー、サインインまたはリスク事象の全体的なリスクのレベルを提供します。 可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。 値`hidden`ユーザーまたはサインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。|
|`riskLevelDuringSignIn`|riskLeve|サインイン中に、(すなわち、リアルタイムのリスク イベントに基づいて) には、サインイン用のリスクのレベルを提供します。 可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。 値`hidden`サインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。|
|`state`|riskState|危険なユーザー、サインインまたはリスク イベントの 'リスク状態' を提供します。 使用可能な値: `none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。 |

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
    "stateDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
    "riskLevelAggregated":  {"@odata.type": "microsoft.graph.riskLevel"},
    "riskLevelDuringSignIn":  {"@odata.type": "microsoft.graph.riskLevel"},
    "state":  {"@odata.type": "microsoft.graph.riskState"}
  }
  ```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/risk.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
