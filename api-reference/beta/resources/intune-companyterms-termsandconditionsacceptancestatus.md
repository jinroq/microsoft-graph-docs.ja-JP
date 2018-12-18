---
title: termsAndConditionsAcceptanceStatus リソース タイプ
description: C) 特定のユーザーがポリシーです。 ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。
author: tfitzmac
ms.openlocfilehash: 8e504796be7dbec303bab8691ed171abc80b9a45
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314638"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a>termsAndConditionsAcceptanceStatus リソース タイプ

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

termsAndConditionsAcceptanceStatus エンティティは、特定のユーザーによる特定の使用条件 (T&C) のポリシーの承諾状況を表します。 ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List termsAndConditionsAcceptanceStatuses](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) コレクション|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|新しい [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを作成します。|
|[Delete termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|なし|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) を削除します。|
|[Update termsAndConditionsAcceptanceStatus](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティの一意識別子。|
|userDisplayName|String|エンティティによって承諾が示されているユーザーの表示名。|
|acceptedVersion|Int32|ユーザーによって承諾された使用条件の最新バージョン番号。|
|acceptedDateTime|DateTimeOffset|最後に使用条件がユーザーによって承諾された DateTime。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|割り当てられた使用条件へのナビゲーション リンク。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```





