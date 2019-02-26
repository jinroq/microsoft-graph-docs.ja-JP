---
title: termsAndConditions リソース タイプ
description: termsAndConditions エンティティは、特定の使用条件 (T&C) ポリシーのメタデータとコンテンツを表します。 T&C ポリシーのコンテンツは、ユーザーが Intune へ最初の登録を試みる際に表示されます。また、その後、管理者が再承認を必要とする編集の際にも表示されます。 それらを使用して、管理者は、デバイスを Intune に登録するためにユーザーが同意しなければならない規定を伝えることができます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9d4366ef5f9e72d6ea3e217fb71eb796bfa20cc
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254780"
---
# <a name="termsandconditions-resource-type"></a>termsAndConditions リソース タイプ

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

termsAndConditions エンティティは、特定の使用条件 (T&C) ポリシーのメタデータとコンテンツを表します。 T&C ポリシーのコンテンツは、ユーザーが Intune へ最初の登録を試みる際に表示されます。また、その後、管理者が再承認を必要とする編集の際にも表示されます。 それらを使用して、管理者は、デバイスを Intune に登録するためにユーザーが同意しなければならない規定を伝えることができます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List termsAndConditionses](../api/intune-companyterms-termsandconditions-list.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) コレクション|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get termsAndConditions](../api/intune-companyterms-termsandconditions-get.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create termsAndConditions](../api/intune-companyterms-termsandconditions-create.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|新しい [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトを作成します。|
|[Delete termsAndConditions](../api/intune-companyterms-termsandconditions-delete.md)|なし|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) を削除します。|
|[Update termsAndConditions](../api/intune-companyterms-termsandconditions-update.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|T&C ポリシーの一意識別子。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。|
|displayName|String|T&C ポリシー用に管理者が提供した名前。 |
|説明|文字列型 (String)|管理者が提供した T&C ポリシーの説明。|
|タイトル|String|管理者が提供した契約条件のタイトル。 ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。|
|bodyText|String|管理者が提供する契約条件の本文で、通常は条件そのものです。 ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。|
|acceptanceStatement|String|使用条件に関する、管理者指定の説明内容です。通常は、T&C ポリシーに定められた使用条件を受け入れることの意味を記載します。 ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。|
|version|Int32|条件の現行バージョンを示す整数。 管理者が使用条件を変更し、修正された T&C ポリシーを再承諾するようにユーザーに求めると、値が増加します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) コレクション|この T&C ポリシーの割り当てのリスト。|
|acceptanceStatuses|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) コレクション|この T&C ポリシーの承諾状態のリスト。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024
}
```



