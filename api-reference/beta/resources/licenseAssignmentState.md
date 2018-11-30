---
title: licenseAssignmentState リソースの種類
description: 'ユーザー エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**のコレクションです。 ユーザー ライセンスの割り当てに関する詳細情報を提供します。 詳細には、ような情報が含まれています。  '
ms.openlocfilehash: 4e7101acc756a845913a081368b79242834ef3bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072227"
---
# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[ユーザー](user.md)エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**のコレクションです。 ユーザー ライセンスの割り当てに関する詳細情報を提供します。 詳細には、ような情報が含まれています。  

 - ユーザーに対してどのようなプランが無効になっています。
 - ライセンスをユーザーに直接割り当てられているか、グループから継承されたかどうか
 - 割り当ての現在の状態
 - 代入の状態がエラーの場合は、エラーのエラーの詳細は? 


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|assignedByGroup|文字列|このライセンスを割り当てられるグループの id。 割り当てがダイレクトに割り当てられたライセンスの場合は、このフィールドは Null になります。 読み取り専用。|
|disabledPlans|Collection(String)|この割り当て内で無効になっているサービス プランです。 読み取り専用。|
|エラー|String|ライセンスの割り当てエラーです。 ライセンスが正常に割り当てられると、このフィールドが Null になります。 読み取り専用。 使用可能な値: `CountViolation`、 `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation`、`UniquenessViolation`と`Others`。 エラーを特定し、ライセンスの割り当てを解決する方法の詳細について参照してください[ここで](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。|
|skuId|String|SKU の一意識別子。 読み取り専用。|
|state|String|この割り当ての現在の状態を示します。 読み取り専用。 使用可能な値: アクティブ、ActiveWithError、無効になり、エラーです。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```