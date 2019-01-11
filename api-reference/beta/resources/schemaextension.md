---
title: schemaExtension リソースの種類 (スキーマ拡張機能)
description: 'スキーマの拡張機能を使用すると、拡張するスキーマを定義し、厳密に型指定されたカスタム データをリソースの種類に追加できます。カスタム データは拡張したリソースの複合型として表示されます。 '
localization_priority: Normal
ms.openlocfilehash: df0b362e87fa0f8cf836c27e89a5fdebd4ab0de8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894503"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="0d345-104">schemaExtension リソースの種類 (スキーマ拡張機能)</span><span class="sxs-lookup"><span data-stu-id="0d345-104">schemaExtension resource type (schema extensions)</span></span>

> <span data-ttu-id="0d345-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0d345-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d345-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d345-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d345-p103">スキーマの拡張機能を使用すると、拡張するスキーマを定義し、厳密に型指定されたカスタム データをリソースの種類に追加できます。カスタム データは拡張したリソースの複合型として表示されます。</span><span class="sxs-lookup"><span data-stu-id="0d345-p103">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="0d345-109">スキーマ拡張機能は次のリソースの種類でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0d345-109">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="0d345-110">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="0d345-110">administrativeUnit</span></span>](administrativeunit.md)
 - [<span data-ttu-id="0d345-111">contact</span><span class="sxs-lookup"><span data-stu-id="0d345-111">contact</span></span>](contact.md)
 - [<span data-ttu-id="0d345-112">device</span><span class="sxs-lookup"><span data-stu-id="0d345-112">device</span></span>](device.md)
 - <span data-ttu-id="0d345-113">ユーザーまたは Office 365 グループ カレンダーの [event](event.md)</span><span class="sxs-lookup"><span data-stu-id="0d345-113">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="0d345-114">Office 365 グループの [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="0d345-114">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="0d345-115">group</span><span class="sxs-lookup"><span data-stu-id="0d345-115">group</span></span>](group.md)
 - [<span data-ttu-id="0d345-116">message</span><span class="sxs-lookup"><span data-stu-id="0d345-116">message</span></span>](message.md) 
 - [<span data-ttu-id="0d345-117">organization</span><span class="sxs-lookup"><span data-stu-id="0d345-117">organization</span></span>](organization.md)
 - [<span data-ttu-id="0d345-118">user</span><span class="sxs-lookup"><span data-stu-id="0d345-118">user</span></span>](user.md)

<span data-ttu-id="0d345-119">カスタム データのグループへの追加方法については、[スキーマ拡張機能の例](/graph/extensibility-schema-groups)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d345-119">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="0d345-120">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d345-120">Methods</span></span>

| <span data-ttu-id="0d345-121">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d345-121">Method</span></span>           | <span data-ttu-id="0d345-122">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0d345-122">Return Type</span></span>    |<span data-ttu-id="0d345-123">説明</span><span class="sxs-lookup"><span data-stu-id="0d345-123">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d345-124">Create</span><span class="sxs-lookup"><span data-stu-id="0d345-124">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="0d345-125">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0d345-125">schemaExtension</span></span> |<span data-ttu-id="0d345-126">スキーマ拡張機能の定義を作成します。</span><span class="sxs-lookup"><span data-stu-id="0d345-126">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="0d345-127">List</span><span class="sxs-lookup"><span data-stu-id="0d345-127">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="0d345-128">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0d345-128">schemaExtension</span></span> |<span data-ttu-id="0d345-129">Avaialbe schemaExtension の定義とそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0d345-129">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="0d345-130">Get</span><span class="sxs-lookup"><span data-stu-id="0d345-130">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="0d345-131">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0d345-131">schemaExtension</span></span> |<span data-ttu-id="0d345-132">特定の schemaExtension 定義のプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0d345-132">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="0d345-133">Update</span><span class="sxs-lookup"><span data-stu-id="0d345-133">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="0d345-134">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0d345-134">schemaExtension</span></span>   |<span data-ttu-id="0d345-135">schemaExtension 定義を更新します。</span><span class="sxs-lookup"><span data-stu-id="0d345-135">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="0d345-136">Delete</span><span class="sxs-lookup"><span data-stu-id="0d345-136">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="0d345-137">なし</span><span class="sxs-lookup"><span data-stu-id="0d345-137">None</span></span> |<span data-ttu-id="0d345-138">schemaExtension 定義を削除します。</span><span class="sxs-lookup"><span data-stu-id="0d345-138">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="0d345-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d345-139">Properties</span></span>
| <span data-ttu-id="0d345-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d345-140">Property</span></span>     | <span data-ttu-id="0d345-141">種類</span><span class="sxs-lookup"><span data-stu-id="0d345-141">Type</span></span>   |<span data-ttu-id="0d345-142">説明</span><span class="sxs-lookup"><span data-stu-id="0d345-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d345-143">説明</span><span class="sxs-lookup"><span data-stu-id="0d345-143">description</span></span>|<span data-ttu-id="0d345-144">String</span><span class="sxs-lookup"><span data-stu-id="0d345-144">String</span></span>|<span data-ttu-id="0d345-145">スキーマ拡張機能の説明。</span><span class="sxs-lookup"><span data-stu-id="0d345-145">Description for the schema extension.</span></span>|
|<span data-ttu-id="0d345-146">id</span><span class="sxs-lookup"><span data-stu-id="0d345-146">id</span></span>|<span data-ttu-id="0d345-147">String</span><span class="sxs-lookup"><span data-stu-id="0d345-147">String</span></span>|<span data-ttu-id="0d345-148">スキーマ拡張機能の定義の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="0d345-148">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="0d345-149">値の割り当ては、以下の 2 方法のいずれかで行うことができます。</span><span class="sxs-lookup"><span data-stu-id="0d345-149">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="0d345-p104">確認されたドメインの内の 1 つの名前とスキーマ拡張機能の名前を連結して、\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\} という形式の一意の文字列を形成します。たとえば、`contoso_mySchema` です。 </span><span class="sxs-lookup"><span data-stu-id="0d345-p104">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="0d345-p105">スキーマ名を指定し、Microsoft Graph がそのスキーマ名を使用して **id** 割り当てを完了するには、次の形式を使用します。ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。たとえば、`extkvbmkofy_mySchema` です。</span><span class="sxs-lookup"><span data-stu-id="0d345-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="0d345-154">作成後、このプロパティは変更できません。</span><span class="sxs-lookup"><span data-stu-id="0d345-154">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="0d345-155">owner</span><span class="sxs-lookup"><span data-stu-id="0d345-155">owner</span></span>|<span data-ttu-id="0d345-156">String</span><span class="sxs-lookup"><span data-stu-id="0d345-156">String</span></span>|<span data-ttu-id="0d345-157">スキーマ拡張機能の所有者であるアプリケーションの `appId` です。</span><span class="sxs-lookup"><span data-stu-id="0d345-157">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="0d345-158">このプロパティは作成時に指定して所有者を設定できます。</span><span class="sxs-lookup"><span data-stu-id="0d345-158">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="0d345-159">指定しない場合、呼び出し元のアプリケーションの `appId` が所有者として設定されます。</span><span class="sxs-lookup"><span data-stu-id="0d345-159">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="0d345-160">どちらの場合も、サインインしたユーザーがアプリケーションの所有者でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="0d345-160">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="0d345-161">設定すると、このプロパティは読み取り専用で、変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="0d345-161">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="0d345-162">properties</span><span class="sxs-lookup"><span data-stu-id="0d345-162">properties</span></span>|<span data-ttu-id="0d345-163">[extensionSchemaProperty](extensionschemaproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0d345-163">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="0d345-164">スキーマ拡張機能の定義を構成するプロパティ名と種類のコレクション。</span><span class="sxs-lookup"><span data-stu-id="0d345-164">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="0d345-165">status</span><span class="sxs-lookup"><span data-stu-id="0d345-165">status</span></span>|<span data-ttu-id="0d345-166">String</span><span class="sxs-lookup"><span data-stu-id="0d345-166">String</span></span>|<span data-ttu-id="0d345-p107">スキーマ拡張機能のライフサイクル状態。考えられる状態は、**InDevelopment**、**Available**、および **Deprecated** です。作成時に自動で **InDevelopment** に設定されます。考えられる状態遷移と動作の詳細については、「[スキーマ拡張機能](/graph/extensibility-overview#schema-extensions)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0d345-p107">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="0d345-171">targetTypes</span><span class="sxs-lookup"><span data-stu-id="0d345-171">targetTypes</span></span>|<span data-ttu-id="0d345-172">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0d345-172">String collection</span></span>|<span data-ttu-id="0d345-173">スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。</span><span class="sxs-lookup"><span data-stu-id="0d345-173">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="0d345-174">**AdministrativeUnit\*\*\*\*にお問い合わせください**、**デバイス**、**イベント**、**グループ**、**メッセージ**、**組織**、**投稿**、または**ユーザー**から選択します。</span><span class="sxs-lookup"><span data-stu-id="0d345-174">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d345-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d345-175">JSON representation</span></span>

<span data-ttu-id="0d345-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0d345-176">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
