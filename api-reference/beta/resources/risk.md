---
title: リソースの種類のリスク
description: レベルのリスク、リスクの状態を集約して、リスクの詳細、リスクの高いユーザーのサインイン、または、イベントのリスクです。
ms.openlocfilehash: bc8ea5c30f78560ae8750e7750596f282feb4825
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069082"
---
# <a name="risk-resource-type"></a>リソースの種類のリスク

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

レベルのリスク、リスクの状態を集約して、リスクの詳細、リスクの高いユーザーのサインイン、または、イベントのリスクです。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|`stateDetail`|riskDetail|危険なユーザー、サインインまたはリスク事象の特定の状態の背後にある '理由' を提供します。 可能な値: `none`、 `adminGeneratedTemporaryPassword`、 `userPerformedSecuredPasswordChange`、 `userPerformedSecuredPasswordReset`、 `adminConfirmedSigninSafe`、 `aiConfirmedSigninSafe`、 `userPassedMFADrivenByRiskBasedPolicy`、 `adminDismissedAllRiskForUser`、 `adminConfirmedSigninCompromised`、 `unknownFutureValue`。 値`none`アクションが実行されたことなしに、ユーザーまたはのサインインでこれまでにすることを意味します。 |
|`riskLevelAggregated`|riskLevel|危険なユーザー、サインインまたはリスク事象の全体的なリスクのレベルを提供します。 可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。 値`hidden`ユーザーまたはサインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。|
|`riskLevelDuringSignIn`|riskLeve|サインイン中に、(すなわち、リアルタイムのリスク イベントに基づいて) には、サインイン用のリスクのレベルを提供します。 可能な値: `none`、 `low`、 `medium`、 `high`、`hidden`と`unknownFutureValue`。 値`hidden`サインインが有効ではなかった Azure AD のアイデンティティ保護のことを意味します。|
|`state`|riskState|危険なユーザー、サインインまたはリスク イベントの 'リスク状態' を提供します。 可能な値: `none`、 `confirmedSafe`、 `remediated`、 `dismissed`、 `atRisk`、 `confirmedCompromised`、 `unknownFutureValue`。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
