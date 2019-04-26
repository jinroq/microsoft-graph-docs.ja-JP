---
title: schemaExtension リソースの種類 (スキーマ拡張機能)
description: 'スキーマの拡張機能を使用すると、拡張するスキーマを定義し、厳密に型指定されたカスタム データをリソースの種類に追加できます。カスタム データは拡張したリソースの複合型として表示されます。 '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: a6d7ed28b1fedefe1b4172bb780e3a014e4d3ff7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343468"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="a7300-104">schemaExtension リソースの種類 (スキーマ拡張機能)</span><span class="sxs-lookup"><span data-stu-id="a7300-104">schemaExtension resource type (schema extensions)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7300-p102">スキーマの拡張機能を使用すると、拡張するスキーマを定義し、厳密に型指定されたカスタム データをリソースの種類に追加できます。カスタム データは拡張したリソースの複合型として表示されます。</span><span class="sxs-lookup"><span data-stu-id="a7300-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="a7300-107">スキーマ拡張機能は次のリソースの種類でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="a7300-107">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="a7300-108">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="a7300-108">administrativeUnit</span></span>](administrativeunit.md)
 - [<span data-ttu-id="a7300-109">contact</span><span class="sxs-lookup"><span data-stu-id="a7300-109">contact</span></span>](contact.md)
 - [<span data-ttu-id="a7300-110">device</span><span class="sxs-lookup"><span data-stu-id="a7300-110">device</span></span>](device.md)
 - <span data-ttu-id="a7300-111">ユーザーまたは Office 365 グループ カレンダーの [event](event.md)</span><span class="sxs-lookup"><span data-stu-id="a7300-111">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="a7300-112">Office 365 グループの [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="a7300-112">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="a7300-113">group</span><span class="sxs-lookup"><span data-stu-id="a7300-113">group</span></span>](group.md)
 - [<span data-ttu-id="a7300-114">message</span><span class="sxs-lookup"><span data-stu-id="a7300-114">message</span></span>](message.md) 
 - [<span data-ttu-id="a7300-115">organization</span><span class="sxs-lookup"><span data-stu-id="a7300-115">organization</span></span>](organization.md)
 - [<span data-ttu-id="a7300-116">user</span><span class="sxs-lookup"><span data-stu-id="a7300-116">user</span></span>](user.md)

<span data-ttu-id="a7300-117">カスタム データのグループへの追加方法については、[スキーマ拡張機能の例](/graph/extensibility-schema-groups)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7300-117">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="a7300-118">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7300-118">Methods</span></span>

| <span data-ttu-id="a7300-119">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7300-119">Method</span></span>           | <span data-ttu-id="a7300-120">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a7300-120">Return Type</span></span>    |<span data-ttu-id="a7300-121">説明</span><span class="sxs-lookup"><span data-stu-id="a7300-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a7300-122">Create</span><span class="sxs-lookup"><span data-stu-id="a7300-122">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="a7300-123">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="a7300-123">schemaExtension</span></span> |<span data-ttu-id="a7300-124">スキーマ拡張機能の定義を作成します。</span><span class="sxs-lookup"><span data-stu-id="a7300-124">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="a7300-125">List</span><span class="sxs-lookup"><span data-stu-id="a7300-125">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="a7300-126">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="a7300-126">schemaExtension</span></span> |<span data-ttu-id="a7300-127">avaialbe schemaextension 日とそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="a7300-127">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="a7300-128">Get</span><span class="sxs-lookup"><span data-stu-id="a7300-128">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="a7300-129">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="a7300-129">schemaExtension</span></span> |<span data-ttu-id="a7300-130">特定の schemaExtension 定義のプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a7300-130">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="a7300-131">Update</span><span class="sxs-lookup"><span data-stu-id="a7300-131">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="a7300-132">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="a7300-132">schemaExtension</span></span>   |<span data-ttu-id="a7300-133">schemaExtension 定義を更新します。</span><span class="sxs-lookup"><span data-stu-id="a7300-133">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="a7300-134">Delete</span><span class="sxs-lookup"><span data-stu-id="a7300-134">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="a7300-135">なし</span><span class="sxs-lookup"><span data-stu-id="a7300-135">None</span></span> |<span data-ttu-id="a7300-136">schemaExtension 定義を削除します。</span><span class="sxs-lookup"><span data-stu-id="a7300-136">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="a7300-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7300-137">Properties</span></span>
| <span data-ttu-id="a7300-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7300-138">Property</span></span>     | <span data-ttu-id="a7300-139">型</span><span class="sxs-lookup"><span data-stu-id="a7300-139">Type</span></span>   |<span data-ttu-id="a7300-140">説明</span><span class="sxs-lookup"><span data-stu-id="a7300-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7300-141">description</span><span class="sxs-lookup"><span data-stu-id="a7300-141">description</span></span>|<span data-ttu-id="a7300-142">String</span><span class="sxs-lookup"><span data-stu-id="a7300-142">String</span></span>|<span data-ttu-id="a7300-143">スキーマ拡張機能の説明。</span><span class="sxs-lookup"><span data-stu-id="a7300-143">Description for the schema extension.</span></span>|
|<span data-ttu-id="a7300-144">id</span><span class="sxs-lookup"><span data-stu-id="a7300-144">id</span></span>|<span data-ttu-id="a7300-145">String</span><span class="sxs-lookup"><span data-stu-id="a7300-145">String</span></span>|<span data-ttu-id="a7300-146">スキーマ拡張機能の定義の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a7300-146">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="a7300-147">値の割り当ては、以下の 2 方法のいずれかで行うことができます。</span><span class="sxs-lookup"><span data-stu-id="a7300-147">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="a7300-p103">確認されたドメインの内の 1 つの名前とスキーマ拡張機能の名前を連結して、\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\} という形式の一意の文字列を形成します。たとえば、`contoso_mySchema` です。 </span><span class="sxs-lookup"><span data-stu-id="a7300-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="a7300-p104">スキーマ名を指定し、Microsoft Graph がそのスキーマ名を使用して **id** 割り当てを完了するには、次の形式を使用します。ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。たとえば、`extkvbmkofy_mySchema` です。</span><span class="sxs-lookup"><span data-stu-id="a7300-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="a7300-152">作成後、このプロパティは変更できません。</span><span class="sxs-lookup"><span data-stu-id="a7300-152">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="a7300-153">owner</span><span class="sxs-lookup"><span data-stu-id="a7300-153">owner</span></span>|<span data-ttu-id="a7300-154">String</span><span class="sxs-lookup"><span data-stu-id="a7300-154">String</span></span>|<span data-ttu-id="a7300-155">スキーマ拡張機能の所有者であるアプリケーションの `appId` です。</span><span class="sxs-lookup"><span data-stu-id="a7300-155">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="a7300-156">このプロパティは作成時に指定して所有者を設定できます。</span><span class="sxs-lookup"><span data-stu-id="a7300-156">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="a7300-157">指定しない場合、呼び出し元のアプリケーションの `appId` が所有者として設定されます。</span><span class="sxs-lookup"><span data-stu-id="a7300-157">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="a7300-158">どちらの場合も、サインインしたユーザーがアプリケーションの所有者でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="a7300-158">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="a7300-159">設定すると、このプロパティは読み取り専用で、変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="a7300-159">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="a7300-160">properties</span><span class="sxs-lookup"><span data-stu-id="a7300-160">properties</span></span>|<span data-ttu-id="a7300-161">[extensionSchemaProperty](extensionschemaproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a7300-161">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="a7300-162">スキーマ拡張機能の定義を構成するプロパティ名と種類のコレクション。</span><span class="sxs-lookup"><span data-stu-id="a7300-162">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="a7300-163">status</span><span class="sxs-lookup"><span data-stu-id="a7300-163">status</span></span>|<span data-ttu-id="a7300-164">String</span><span class="sxs-lookup"><span data-stu-id="a7300-164">String</span></span>|<span data-ttu-id="a7300-165">スキーマ拡張機能のライフサイクル状態。</span><span class="sxs-lookup"><span data-stu-id="a7300-165">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="a7300-166">考えられる状態は、**InDevelopment**、**Available**、および **Deprecated** です。</span><span class="sxs-lookup"><span data-stu-id="a7300-166">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="a7300-167">作成時に自動で **InDevelopment** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="a7300-167">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="a7300-168">考えられる状態遷移と動作の詳細については、「[スキーマ拡張機能](/graph/extensibility-overview#schema-extensions)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a7300-168">[Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="a7300-169">targetTypes</span><span class="sxs-lookup"><span data-stu-id="a7300-169">targetTypes</span></span>|<span data-ttu-id="a7300-170">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a7300-170">String collection</span></span>|<span data-ttu-id="a7300-171">スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。</span><span class="sxs-lookup"><span data-stu-id="a7300-171">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="a7300-172">**administrativeUnit**、**連絡先**、**デバイス**、**イベント**、**グループ**、**メッセージ**、**組織**、**投稿**、**ユーザー**のいずれかを選択します。</span><span class="sxs-lookup"><span data-stu-id="a7300-172">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7300-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7300-173">JSON representation</span></span>

<span data-ttu-id="a7300-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a7300-174">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
