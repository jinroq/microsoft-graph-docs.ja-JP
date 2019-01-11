---
title: リソースの種類のリスク
description: レベルのリスク、リスクの状態を集約して、リスクの詳細、リスクの高いユーザーのサインイン、または、イベントのリスクです。
localization_priority: Normal
ms.openlocfilehash: da198ba27ca6cd0b762f322863f8c9bfd56a5cb7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810669"
---
# <a name="risk-resource-type"></a>リソースの種類のリスク

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

レベルのリスク、リスクの状態を集約して、リスクの詳細、リスクの高いユーザーのサインイン、または、イベントのリスクです。

## <a name="properties"></a>プロパティ

| プロパティ   | 種類|説明|
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
