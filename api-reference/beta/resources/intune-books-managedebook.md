---
title: managedEBook リソースの種類
description: 管理対象電子ブックの基本プロパティを含む抽象クラスです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8bf13e2c0a5c8e55a397516c21fe91d65aa413a5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991654"
---
# <a name="managedebook-resource-type"></a>managedEBook リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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
|id|文字列|エンティティのキー。|
|displayName|String|電子ブックの名前。|
|description|文字列型 (String)|説明。|
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
|categories|[Managedebookcategory](../resources/intune-books-managedebookcategory.md)コレクション|この電子ブックのカテゴリのリスト。|
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





