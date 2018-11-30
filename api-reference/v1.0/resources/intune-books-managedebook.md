---
title: managedEBook リソースの種類
description: 管理対象電子ブックの基本プロパティを含む抽象クラスです。
ms.openlocfilehash: 427582977558254561b219dff2392f01ced4f53d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023486"
---
# <a name="managedebook-resource-type"></a>managedEBook リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理対象電子ブックの基本プロパティを含む抽象クラスです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managedEBook のリスト](../api/intune-books-managedebook-list.md)|[managedEBook](../resources/intune-books-managedebook.md) コレクション|[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[managedEBook の取得](../api/intune-books-managedebook-get.md)|[managedEBook](../resources/intune-books-managedebook.md)|[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[アクションの割り当て](../api/intune-books-managedebook-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|displayName|String|電子ブックの名前。|
|説明|String|説明。|
|publisher|String|発行元です。|
|publishedDateTime|DateTimeOffset|電子ブックが発行された日時。|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|ブック カバー。|
|createdDateTime|DateTimeOffset|電子ブック ファイルが作成された日時。|
|lastModifiedDateTime|DateTimeOffset|電子ブックが最後に変更された日時。|
|informationUrl|String|詳細情報の URL。|
|privacyInformationUrl|String|プライバシーに関する声明の URL。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション|この電子ブックの割り当てのリストです。|
|installSummary|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|モバイル アプリ インストール概要です。|
|deviceStates|[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション|この電子ブックのインストール状態のリストです。|
|userStateSummary|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション|この電子ブックのインストール状態のリストです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



