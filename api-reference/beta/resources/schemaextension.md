---
title: schemaExtension リソースの種類 (スキーマ拡張機能)
description: 'スキーマの拡張機能を使用すると、拡張するスキーマを定義し、厳密に型指定されたカスタム データをリソースの種類に追加できます。カスタム データは拡張したリソースの複合型として表示されます。 '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 90acbfb0e7a6b031303ae3286f1a5ed366a2a8c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523856"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="5bd9c-104">schemaExtension リソースの種類 (スキーマ拡張機能)</span><span class="sxs-lookup"><span data-stu-id="5bd9c-104">schemaExtension resource type (schema extensions)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bd9c-p102">スキーマの拡張機能を使用すると、拡張するスキーマを定義し、厳密に型指定されたカスタム データをリソースの種類に追加できます。カスタム データは拡張したリソースの複合型として表示されます。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="5bd9c-107">スキーマ拡張機能は次のリソースの種類でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-107">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="5bd9c-108">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="5bd9c-108">administrativeUnit</span></span>](administrativeunit.md)
 - [<span data-ttu-id="5bd9c-109">contact</span><span class="sxs-lookup"><span data-stu-id="5bd9c-109">contact</span></span>](contact.md)
 - [<span data-ttu-id="5bd9c-110">device</span><span class="sxs-lookup"><span data-stu-id="5bd9c-110">device</span></span>](device.md)
 - <span data-ttu-id="5bd9c-111">ユーザーまたは Office 365 グループ カレンダーの [event](event.md)</span><span class="sxs-lookup"><span data-stu-id="5bd9c-111">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="5bd9c-112">Office 365 グループの [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="5bd9c-112">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="5bd9c-113">group</span><span class="sxs-lookup"><span data-stu-id="5bd9c-113">group</span></span>](group.md)
 - [<span data-ttu-id="5bd9c-114">message</span><span class="sxs-lookup"><span data-stu-id="5bd9c-114">message</span></span>](message.md) 
 - [<span data-ttu-id="5bd9c-115">organization</span><span class="sxs-lookup"><span data-stu-id="5bd9c-115">organization</span></span>](organization.md)
 - [<span data-ttu-id="5bd9c-116">user</span><span class="sxs-lookup"><span data-stu-id="5bd9c-116">user</span></span>](user.md)

<span data-ttu-id="5bd9c-117">カスタム データのグループへの追加方法については、[スキーマ拡張機能の例](/graph/extensibility-schema-groups)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-117">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="5bd9c-118">メソッド</span><span class="sxs-lookup"><span data-stu-id="5bd9c-118">Methods</span></span>

| <span data-ttu-id="5bd9c-119">メソッド</span><span class="sxs-lookup"><span data-stu-id="5bd9c-119">Method</span></span>           | <span data-ttu-id="5bd9c-120">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5bd9c-120">Return Type</span></span>    |<span data-ttu-id="5bd9c-121">説明</span><span class="sxs-lookup"><span data-stu-id="5bd9c-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5bd9c-122">Create</span><span class="sxs-lookup"><span data-stu-id="5bd9c-122">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="5bd9c-123">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="5bd9c-123">schemaExtension</span></span> |<span data-ttu-id="5bd9c-124">スキーマ拡張機能の定義を作成します。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-124">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="5bd9c-125">List</span><span class="sxs-lookup"><span data-stu-id="5bd9c-125">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="5bd9c-126">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="5bd9c-126">schemaExtension</span></span> |<span data-ttu-id="5bd9c-127">Avaialbe schemaExtension の定義とそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-127">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="5bd9c-128">Get</span><span class="sxs-lookup"><span data-stu-id="5bd9c-128">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="5bd9c-129">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="5bd9c-129">schemaExtension</span></span> |<span data-ttu-id="5bd9c-130">特定の schemaExtension 定義のプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-130">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="5bd9c-131">Update</span><span class="sxs-lookup"><span data-stu-id="5bd9c-131">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="5bd9c-132">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="5bd9c-132">schemaExtension</span></span>   |<span data-ttu-id="5bd9c-133">schemaExtension 定義を更新します。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-133">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="5bd9c-134">Delete</span><span class="sxs-lookup"><span data-stu-id="5bd9c-134">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="5bd9c-135">なし</span><span class="sxs-lookup"><span data-stu-id="5bd9c-135">None</span></span> |<span data-ttu-id="5bd9c-136">schemaExtension 定義を削除します。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-136">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="5bd9c-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5bd9c-137">Properties</span></span>
| <span data-ttu-id="5bd9c-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5bd9c-138">Property</span></span>     | <span data-ttu-id="5bd9c-139">型</span><span class="sxs-lookup"><span data-stu-id="5bd9c-139">Type</span></span>   |<span data-ttu-id="5bd9c-140">説明</span><span class="sxs-lookup"><span data-stu-id="5bd9c-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bd9c-141">説明</span><span class="sxs-lookup"><span data-stu-id="5bd9c-141">description</span></span>|<span data-ttu-id="5bd9c-142">文字列</span><span class="sxs-lookup"><span data-stu-id="5bd9c-142">String</span></span>|<span data-ttu-id="5bd9c-143">スキーマ拡張機能の説明。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-143">Description for the schema extension.</span></span>|
|<span data-ttu-id="5bd9c-144">id</span><span class="sxs-lookup"><span data-stu-id="5bd9c-144">id</span></span>|<span data-ttu-id="5bd9c-145">文字列</span><span class="sxs-lookup"><span data-stu-id="5bd9c-145">String</span></span>|<span data-ttu-id="5bd9c-146">スキーマ拡張機能の定義の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-146">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="5bd9c-147">値の割り当ては、以下の 2 方法のいずれかで行うことができます。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-147">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="5bd9c-p103">確認されたドメインの内の 1 つの名前とスキーマ拡張機能の名前を連結して、\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\} という形式の一意の文字列を形成します。たとえば、`contoso_mySchema` です。 </span><span class="sxs-lookup"><span data-stu-id="5bd9c-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="5bd9c-p104">スキーマ名を指定し、Microsoft Graph がそのスキーマ名を使用して **id** 割り当てを完了するには、次の形式を使用します。ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。たとえば、`extkvbmkofy_mySchema` です。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="5bd9c-152">作成後、このプロパティは変更できません。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-152">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="5bd9c-153">owner</span><span class="sxs-lookup"><span data-stu-id="5bd9c-153">owner</span></span>|<span data-ttu-id="5bd9c-154">String</span><span class="sxs-lookup"><span data-stu-id="5bd9c-154">String</span></span>|<span data-ttu-id="5bd9c-155">スキーマ拡張機能の所有者であるアプリケーションの `appId` です。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-155">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="5bd9c-156">このプロパティは作成時に指定して所有者を設定できます。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-156">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="5bd9c-157">指定しない場合、呼び出し元のアプリケーションの `appId` が所有者として設定されます。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-157">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="5bd9c-158">どちらの場合も、サインインしたユーザーがアプリケーションの所有者でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-158">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="5bd9c-159">設定すると、このプロパティは読み取り専用で、変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-159">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="5bd9c-160">properties</span><span class="sxs-lookup"><span data-stu-id="5bd9c-160">properties</span></span>|<span data-ttu-id="5bd9c-161">[extensionSchemaProperty](extensionschemaproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5bd9c-161">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="5bd9c-162">スキーマ拡張機能の定義を構成するプロパティ名と種類のコレクション。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-162">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="5bd9c-163">status</span><span class="sxs-lookup"><span data-stu-id="5bd9c-163">status</span></span>|<span data-ttu-id="5bd9c-164">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5bd9c-164">String</span></span>|<span data-ttu-id="5bd9c-p106">スキーマ拡張機能のライフサイクル状態。考えられる状態は、**InDevelopment**、**Available**、および **Deprecated** です。作成時に自動で **InDevelopment** に設定されます。考えられる状態遷移と動作の詳細については、「[スキーマ拡張機能](/graph/extensibility-overview#schema-extensions)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-p106">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="5bd9c-169">targetTypes</span><span class="sxs-lookup"><span data-stu-id="5bd9c-169">targetTypes</span></span>|<span data-ttu-id="5bd9c-170">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5bd9c-170">String collection</span></span>|<span data-ttu-id="5bd9c-171">スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-171">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="5bd9c-172">**AdministrativeUnit\*\*\*\*にお問い合わせください**、**デバイス**、**イベント**、**グループ**、**メッセージ**、**組織**、**投稿**、または**ユーザー**から選択します。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-172">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5bd9c-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5bd9c-173">JSON representation</span></span>

<span data-ttu-id="5bd9c-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5bd9c-174">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/schemaextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
