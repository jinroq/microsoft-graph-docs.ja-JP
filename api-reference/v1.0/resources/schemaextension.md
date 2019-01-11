---
title: schemaExtension リソースの種類 (スキーマ拡張機能)
description: 'スキーマの拡張機能を使用すると、拡張するスキーマを定義し、厳密に型指定されたカスタム データをリソースの種類に追加できます。カスタム データは拡張したリソースの複合型として表示されます。 '
localization_priority: Priority
ms.openlocfilehash: 9a21989aa2c5c7cf8c83873286b800b748097bf1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877008"
---
# <a name="schemaextension-resource-type-schema-extensions"></a>schemaExtension リソースの種類 (スキーマ拡張機能)

スキーマの拡張機能を使用すると、拡張するスキーマを定義し、厳密に型指定されたカスタム データをリソースの種類に追加できます。カスタム データは拡張したリソースの複合型として表示されます。 

スキーマ拡張機能は次のリソースの種類でサポートされています。

 - [contact](contact.md)
 - [device](device.md)
 - ユーザーまたは Office 365 グループ カレンダーの [event](event.md)
 - Office 365 グループの [post](post.md)
 - [group](group.md)
 - [message](message.md) 
 - [organization](organization.md)
 - [user](user.md)

カスタム データのグループへの追加方法については、[スキーマ拡張機能の例](/graph/extensibility-schema-groups)を参照してください。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Create](../api/schemaextension-post-schemaextensions.md) | schemaExtension |スキーマ拡張機能の定義を作成します。|
|[List](../api/schemaextension-list.md) | schemaExtension |使用可能な schemaExtension の定義とそのプロパティを一覧表示します。|
|[Get](../api/schemaextension-get.md) | schemaExtension |特定の schemaExtension 定義のプロパティを読み取ります。|
|[Update](../api/schemaextension-update.md) | schemaExtension   |schemaExtension 定義を更新します。 |
|[Delete](../api/schemaextension-delete.md) | なし |schemaExtension 定義を削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|説明|String|スキーマ拡張機能の説明。|
|id|String|スキーマ拡張機能の定義の一意の識別子。 <br>値の割り当ては、以下の 2 方法のいずれかで行うことができます。 <ul><li>確認されたドメインの内の 1 つの名前とスキーマ拡張機能の名前を連結して、\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\} という形式の一意の文字列を形成します。たとえば、`contoso_mySchema` です。 </li><li>スキーマ名を指定し、Microsoft Graph がそのスキーマ名を使用して **id** 割り当てを完了するには、次の形式を使用します。ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。たとえば、`extkvbmkofy_mySchema` です。</li></ul>作成後、このプロパティは変更できません。 |
|owner|String|スキーマ拡張機能の所有者であるアプリケーションの `appId` です。 このプロパティは作成時に指定して所有者を設定できます。  指定しない場合、呼び出し元のアプリケーションの `appId` が所有者として設定されます。 どちらの場合も、サインインしたユーザーがアプリケーションの所有者でなければなりません。 設定すると、このプロパティは読み取り専用で、変更することはできません。| 
|properties|[extensionSchemaProperty](extensionschemaproperty.md) コレクション|スキーマ拡張機能の定義を構成するプロパティ名と種類のコレクション。|
|status|String|スキーマ拡張機能のライフサイクル状態。考えられる状態は、**InDevelopment**、**Available**、および **Deprecated** です。作成時に自動で **InDevelopment** に設定されます。考えられる状態遷移と動作の詳細については、「[スキーマ拡張機能](/graph/extensibility-overview#schema-extensions)」をご覧ください。|
|targetTypes|String コレクション|スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。**contact**、**device**、**event**、**group**、**message**、**organization**、**post**、**user** のいずれかから選択します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
