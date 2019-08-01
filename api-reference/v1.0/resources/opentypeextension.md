---
title: openTypeExtension リソース タイプ (オープン拡張機能)
description: オープン拡張 (旧称は Office 365 のデータ拡張機能) を使用すると、型指定されていないプロパティを Microsoft Graph のリソースに簡単に直接追加できます。
localization_priority: Priority
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 51633d9d166d28033f49463176232c62aa557c59
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035746"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="02a83-103">openTypeExtension リソース タイプ (オープン拡張)</span><span class="sxs-lookup"><span data-stu-id="02a83-103">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="02a83-104">オープン拡張 (旧称は Office 365 のデータ拡張機能) を使用すると、型指定されていないプロパティを Microsoft Graph のリソースに簡単に直接追加できます。</span><span class="sxs-lookup"><span data-stu-id="02a83-104">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>

<span data-ttu-id="02a83-105">オープン拡張機能は、**openTypeExtension** リソースで表されます。</span><span class="sxs-lookup"><span data-stu-id="02a83-105">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="02a83-106">リソースに追加されるオープン拡張機能は **extensions** ナビゲーション プロパティに表示されます。このプロパティは、[extension](extension.md) 抽象型から派生します。</span><span class="sxs-lookup"><span data-stu-id="02a83-106">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span> <span data-ttu-id="02a83-107">各拡張機能には **extensionName** プロパティがあります。このプロパティは、すべての拡張機能とカスタム データで唯一定義済みの書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="02a83-107">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span>

<span data-ttu-id="02a83-108">拡張機能名が必ず一意であるようにする方法の 1 つは、_独自のドメイン_に依存する逆引きドメイン ネーム システム (DNS) 形式 (例: `Com.Contoso.ContactInfo`) を使用することです。</span><span class="sxs-lookup"><span data-stu-id="02a83-108">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="02a83-109">拡張機能名に Microsoft ドメイン (`Com.Microsoft` または `Com.OnMicrosoft`) を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="02a83-109">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="02a83-110">オープン拡張機能の例:[オープン拡張機能を使用したユーザーへのカスタム データの追加](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="02a83-110">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="02a83-111">オープン拡張機能は、次のリソースの対応するバージョンの一般提供 (GA: /v1.0 および /ベータ) またはプレビュー (/ベータ) でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="02a83-111">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

|<span data-ttu-id="02a83-112">リソース</span><span class="sxs-lookup"><span data-stu-id="02a83-112">Resource</span></span> |<span data-ttu-id="02a83-113">バージョン</span><span class="sxs-lookup"><span data-stu-id="02a83-113">Version</span></span> |
|:---------------|:-------|
| [<span data-ttu-id="02a83-114">管理単位</span><span class="sxs-lookup"><span data-stu-id="02a83-114">Administrative unit</span></span>](/graph/api/resources/administrativeunit?view=graph-rest-beta)  | <span data-ttu-id="02a83-115">プレビューのみ</span><span class="sxs-lookup"><span data-stu-id="02a83-115">Preview only</span></span> |
| [<span data-ttu-id="02a83-116">予定表イベント</span><span class="sxs-lookup"><span data-stu-id="02a83-116">Calendar event</span></span>](event.md) | <span data-ttu-id="02a83-117">GA</span><span class="sxs-lookup"><span data-stu-id="02a83-117">GA</span></span> |
| <span data-ttu-id="02a83-118">グループ[予定表イベント](event.md)</span><span class="sxs-lookup"><span data-stu-id="02a83-118">Group [calendar event](event.md)</span></span> | <span data-ttu-id="02a83-119">GA</span><span class="sxs-lookup"><span data-stu-id="02a83-119">GA</span></span> |
| <span data-ttu-id="02a83-120">グループ会話スレッド[投稿](post.md)</span><span class="sxs-lookup"><span data-stu-id="02a83-120">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="02a83-121">GA</span><span class="sxs-lookup"><span data-stu-id="02a83-121">GA</span></span> |
| [<span data-ttu-id="02a83-122">device</span><span class="sxs-lookup"><span data-stu-id="02a83-122">device</span></span>](device.md) | <span data-ttu-id="02a83-123">GA</span><span class="sxs-lookup"><span data-stu-id="02a83-123">GA</span></span> |
| [<span data-ttu-id="02a83-124">グループ</span><span class="sxs-lookup"><span data-stu-id="02a83-124">group</span></span>](group.md) | <span data-ttu-id="02a83-125">GA</span><span class="sxs-lookup"><span data-stu-id="02a83-125">GA</span></span> |
| [<span data-ttu-id="02a83-126">メッセージ</span><span class="sxs-lookup"><span data-stu-id="02a83-126">message</span></span>](message.md) | <span data-ttu-id="02a83-127">GA</span><span class="sxs-lookup"><span data-stu-id="02a83-127">GA</span></span> |
| [<span data-ttu-id="02a83-128">組織</span><span class="sxs-lookup"><span data-stu-id="02a83-128">organization</span></span>](organization.md) | <span data-ttu-id="02a83-129">GA</span><span class="sxs-lookup"><span data-stu-id="02a83-129">GA</span></span> |
| [<span data-ttu-id="02a83-130">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="02a83-130">Personal contact</span></span>](contact.md) | <span data-ttu-id="02a83-131">GA</span><span class="sxs-lookup"><span data-stu-id="02a83-131">GA</span></span> |
| [<span data-ttu-id="02a83-132">ユーザー</span><span class="sxs-lookup"><span data-stu-id="02a83-132">user</span></span>](user.md) | <span data-ttu-id="02a83-133">GA</span><span class="sxs-lookup"><span data-stu-id="02a83-133">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="02a83-134">Outlook 固有の考慮事項</span><span class="sxs-lookup"><span data-stu-id="02a83-134">Outlook-specific considerations</span></span>

<span data-ttu-id="02a83-135">Outlook リソース (イベント、メッセージ、個人用連絡先) に存在する各オープン拡張は、[MAPI 名前付きプロパティ](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)に保存されます。</span><span class="sxs-lookup"><span data-stu-id="02a83-135">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="02a83-136">Outlook のオープン拡張を作成する場合は、MAPI 名前付きプロパティがユーザーのメールボックスで有限のリソースであることを考慮してください。</span><span class="sxs-lookup"><span data-stu-id="02a83-136">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="02a83-137">ユーザーの名前付きプロパティのクォータがすべて使用されると、それ以上、そのユーザーに対して名前付きのプロパティを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="02a83-137">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="02a83-138">これにより、機能する名前付きプロパティに依存しているクライアントから、予期しない動作が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="02a83-138">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="02a83-139">Outlook リソースのオープン拡張を作成する場合は、次のガイドラインを適用します。</span><span class="sxs-lookup"><span data-stu-id="02a83-139">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="02a83-140">必要な拡張機能の最小数を作成します。</span><span class="sxs-lookup"><span data-stu-id="02a83-140">Create the minimum number of extensions required.</span></span> <span data-ttu-id="02a83-141">ほとんどのアプリケーションで必要な拡張機能は、1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="02a83-141">Most applications should require no more than one extension.</span></span> <span data-ttu-id="02a83-142">拡張機能には、定義済みのプロパティや構造体が設定されていないため、1 つの拡張機能に複数の値を保存できます。</span><span class="sxs-lookup"><span data-stu-id="02a83-142">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="02a83-143">拡張機能には変更可能な方法 (ユーザー入力に基づくなど) で名前を付けないでください。</span><span class="sxs-lookup"><span data-stu-id="02a83-143">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="02a83-144">ユーザーのメールボックスで以前に使用されていない新しい名前でオープン拡張が作成されるたびに、新しい MAPI 名前付きプロパティが作成されます。</span><span class="sxs-lookup"><span data-stu-id="02a83-144">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="02a83-145">拡張機能を削除しても、名前付きプロパティは削除されません。</span><span class="sxs-lookup"><span data-stu-id="02a83-145">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="02a83-146">オープン拡張 (Outlook リソース用) または拡張プロパティを使用する</span><span class="sxs-lookup"><span data-stu-id="02a83-146">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="02a83-147">オープン拡張は、カスタム データの保存およびカスタム データへのアクセスを必要とするほとんどのシナリオに対して推奨されるソリューションです。</span><span class="sxs-lookup"><span data-stu-id="02a83-147">Open extensions are the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="02a83-148">ただし、[拡張プロパティとこの REST API](extended-properties-overview.md) は、[Microsoft Graph API のメタデータ](https://developer.microsoft.com/graph/docs/overview/call_api)を通じてまだ公開されていない Outlook MAPI プロパティのカスタム データにアクセスする必要がある場合に使用できます。</span><span class="sxs-lookup"><span data-stu-id="02a83-148">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="02a83-149">メタデータが公開するプロパティは、[https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata) で確認できます。</span><span class="sxs-lookup"><span data-stu-id="02a83-149">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="02a83-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02a83-150">JSON representation</span></span>

<span data-ttu-id="02a83-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="02a83-151">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.extension",
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a><span data-ttu-id="02a83-152">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02a83-152">Properties</span></span>

|<span data-ttu-id="02a83-153">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02a83-153">Property</span></span> | <span data-ttu-id="02a83-154">型</span><span class="sxs-lookup"><span data-stu-id="02a83-154">Type</span></span> | <span data-ttu-id="02a83-155">説明</span><span class="sxs-lookup"><span data-stu-id="02a83-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="02a83-156">extensionName</span><span class="sxs-lookup"><span data-stu-id="02a83-156">extensionName</span></span>|<span data-ttu-id="02a83-157">String</span><span class="sxs-lookup"><span data-stu-id="02a83-157">String</span></span>|<span data-ttu-id="02a83-p107">オープン型のオープン拡張機能の一意のテキスト識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="02a83-p107">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="02a83-160">id</span><span class="sxs-lookup"><span data-stu-id="02a83-160">id</span></span>|<span data-ttu-id="02a83-161">String</span><span class="sxs-lookup"><span data-stu-id="02a83-161">String</span></span>| <span data-ttu-id="02a83-p108">**extensionName** と拡張子タイプを連結する完全修飾識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="02a83-p108">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02a83-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="02a83-164">Relationships</span></span>

<span data-ttu-id="02a83-165">なし</span><span class="sxs-lookup"><span data-stu-id="02a83-165">None</span></span>

## <a name="methods"></a><span data-ttu-id="02a83-166">メソッド</span><span class="sxs-lookup"><span data-stu-id="02a83-166">Methods</span></span>

|<span data-ttu-id="02a83-167">メソッド</span><span class="sxs-lookup"><span data-stu-id="02a83-167">Method</span></span> | <span data-ttu-id="02a83-168">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="02a83-168">Return Type</span></span> | <span data-ttu-id="02a83-169">説明</span><span class="sxs-lookup"><span data-stu-id="02a83-169">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="02a83-170">Post</span><span class="sxs-lookup"><span data-stu-id="02a83-170">Post</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="02a83-171">(既存リソースのインスタンス内の) [openTypeExtension](opentypeextension.md)、または、openTypeExtension オブジェクトを含む新しい[contact](../resources/contact.md)、[event](../resources/event.md)、[message](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="02a83-171">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object</span></span> | <span data-ttu-id="02a83-172">既存または新規のリソース インスタンス内に openTypeExtension オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="02a83-172">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="02a83-173">Get</span><span class="sxs-lookup"><span data-stu-id="02a83-173">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="02a83-174">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="02a83-174">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="02a83-175">openTypeExtension オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="02a83-175">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="02a83-176">更新する</span><span class="sxs-lookup"><span data-stu-id="02a83-176">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="02a83-177">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="02a83-177">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="02a83-178">openTypeExtension オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="02a83-178">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="02a83-179">削除</span><span class="sxs-lookup"><span data-stu-id="02a83-179">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="02a83-180">なし</span><span class="sxs-lookup"><span data-stu-id="02a83-180">None</span></span> |<span data-ttu-id="02a83-181">openTypeExtension オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="02a83-181">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
