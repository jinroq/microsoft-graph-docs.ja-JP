---
title: openTypeExtension リソース タイプ (オープン拡張機能)
description: (Office 365 のデータ拡張機能と呼ばれていました) 開いているの拡張機能では、直接グラフ内のリソースに型指定されていないプロパティを追加する簡単な方法を提供します。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: ba5dbcd6c5ae1705ffe7e89ca6f529280d98adf5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508833"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="75308-103">openTypeExtension リソース タイプ (オープン拡張機能)</span><span class="sxs-lookup"><span data-stu-id="75308-103">openTypeExtension resource type (open extensions)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75308-104">(Office 365 のデータ拡張機能と呼ばれていました) 開いているの拡張機能では、直接グラフ内のリソースに型指定されていないプロパティを追加する簡単な方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="75308-104">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>
<span data-ttu-id="75308-105">オープン拡張機能は、**openTypeExtension** リソースで表されます。</span><span class="sxs-lookup"><span data-stu-id="75308-105">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="75308-106">リソースに追加されるオープン拡張機能は **extensions** ナビゲーション プロパティに表示されます。このプロパティは、[extension](extension.md) 抽象型から派生します。</span><span class="sxs-lookup"><span data-stu-id="75308-106">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span>  <span data-ttu-id="75308-107">各拡張機能には **extensionName** プロパティがあります。このプロパティは、すべての拡張機能とカスタム データで唯一定義済みの書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="75308-107">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> <span data-ttu-id="75308-108">拡張機能名が必ず一意であるようにする方法の 1 つは、_独自のドメイン_に依存する逆引きドメイン ネーム システム (DNS) 形式 (例: `Com.Contoso.ContactInfo`) を使用することです。</span><span class="sxs-lookup"><span data-stu-id="75308-108">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="75308-109">拡張機能名に Microsoft ドメイン (`Com.Microsoft` または `Com.OnMicrosoft`) を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="75308-109">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="75308-110">オープン拡張機能の例:[オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="75308-110">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="75308-111">オープン拡張機能は、次のリソースの対応するバージョンの一般提供 (GA: /v1.0 および /ベータ) またはプレビュー (/ベータ) でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="75308-111">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="75308-112">リソース</span><span class="sxs-lookup"><span data-stu-id="75308-112">Resource</span></span> | <span data-ttu-id="75308-113">バージョン</span><span class="sxs-lookup"><span data-stu-id="75308-113">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="75308-114">管理単位</span><span class="sxs-lookup"><span data-stu-id="75308-114">Administrative unit</span></span>](administrativeunit.md)  | <span data-ttu-id="75308-115">プレビューのみ</span><span class="sxs-lookup"><span data-stu-id="75308-115">Preview only</span></span> |
| [<span data-ttu-id="75308-116">予定表イベント</span><span class="sxs-lookup"><span data-stu-id="75308-116">Calendar event</span></span>](event.md) | <span data-ttu-id="75308-117">GA</span><span class="sxs-lookup"><span data-stu-id="75308-117">GA</span></span> |
| <span data-ttu-id="75308-118">グループ[予定表イベント](event.md)</span><span class="sxs-lookup"><span data-stu-id="75308-118">Group [calendar event](event.md)</span></span> | <span data-ttu-id="75308-119">GA</span><span class="sxs-lookup"><span data-stu-id="75308-119">GA</span></span> |
| <span data-ttu-id="75308-120">グループ会話スレッド[投稿](post.md)</span><span class="sxs-lookup"><span data-stu-id="75308-120">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="75308-121">GA</span><span class="sxs-lookup"><span data-stu-id="75308-121">GA</span></span> |
| [<span data-ttu-id="75308-122">device</span><span class="sxs-lookup"><span data-stu-id="75308-122">device</span></span>](device.md) | <span data-ttu-id="75308-123">GA</span><span class="sxs-lookup"><span data-stu-id="75308-123">GA</span></span> |
| [<span data-ttu-id="75308-124">グループ</span><span class="sxs-lookup"><span data-stu-id="75308-124">group</span></span>](group.md) | <span data-ttu-id="75308-125">GA</span><span class="sxs-lookup"><span data-stu-id="75308-125">GA</span></span> |
| [<span data-ttu-id="75308-126">メッセージ</span><span class="sxs-lookup"><span data-stu-id="75308-126">message</span></span>](message.md) | <span data-ttu-id="75308-127">GA</span><span class="sxs-lookup"><span data-stu-id="75308-127">GA</span></span> |
| [<span data-ttu-id="75308-128">組織</span><span class="sxs-lookup"><span data-stu-id="75308-128">organization</span></span>](organization.md) | <span data-ttu-id="75308-129">GA</span><span class="sxs-lookup"><span data-stu-id="75308-129">GA</span></span> |
| [<span data-ttu-id="75308-130">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="75308-130">Personal contact</span></span>](contact.md) | <span data-ttu-id="75308-131">GA</span><span class="sxs-lookup"><span data-stu-id="75308-131">GA</span></span> |
| [<span data-ttu-id="75308-132">ユーザー</span><span class="sxs-lookup"><span data-stu-id="75308-132">user</span></span>](user.md) | <span data-ttu-id="75308-133">GA</span><span class="sxs-lookup"><span data-stu-id="75308-133">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="75308-134">Outlook に固有の考慮事項</span><span class="sxs-lookup"><span data-stu-id="75308-134">Outlook-specific considerations</span></span>

<span data-ttu-id="75308-135">(イベント、メッセージ、または個人用の連絡先)、Outlook のリソース上に存在の開いている各拡張機能は、 [MAPI の名前付きプロパティ](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)に格納されます。</span><span class="sxs-lookup"><span data-stu-id="75308-135">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="75308-136">Outlook を開いている拡張機能を作成するときは、MAPI プロパティを名前付きのユーザーのメールボックス内の有限のリソースであることを検討します。</span><span class="sxs-lookup"><span data-stu-id="75308-136">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="75308-137">ユーザーの名前付きプロパティのクォータが不足すると、そのユーザーに対して複数の名前付きプロパティを作成できません。</span><span class="sxs-lookup"><span data-stu-id="75308-137">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="75308-138">その場合、関数の名前付きプロパティに依存するクライアントからの予期しない動作します。</span><span class="sxs-lookup"><span data-stu-id="75308-138">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="75308-139">Outlook のリソースで開いている拡張機能を作成するときは、次のガイドラインを適用します。</span><span class="sxs-lookup"><span data-stu-id="75308-139">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="75308-140">必要な拡張の最小数を作成します。</span><span class="sxs-lookup"><span data-stu-id="75308-140">Create the minimum number of extensions required.</span></span> <span data-ttu-id="75308-141">ほとんどのアプリケーションは、複数の拡張機能を必要があります。</span><span class="sxs-lookup"><span data-stu-id="75308-141">Most applications should require no more than one extension.</span></span> <span data-ttu-id="75308-142">拡張機能があるないプロパティの設定を定義または構造体は、単一の拡張機能に複数の値を格納することができますので。</span><span class="sxs-lookup"><span data-stu-id="75308-142">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="75308-143">(などのユーザー入力などに基づきます)。 変数の方法で拡張機能の名前付けをしないでください。</span><span class="sxs-lookup"><span data-stu-id="75308-143">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="75308-144">前に、ユーザーのメールボックスで使用されていない新しい名前で開いている拡張機能を作成するたびに、新しい MAPI 名前付きプロパティが作成されます。</span><span class="sxs-lookup"><span data-stu-id="75308-144">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="75308-145">拡張子を削除しても、名前付きプロパティは削除されません。</span><span class="sxs-lookup"><span data-stu-id="75308-145">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="75308-146">オープン拡張機能 (Outlook リソース用) と拡張プロパティのどちらを使用するか</span><span class="sxs-lookup"><span data-stu-id="75308-146">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="75308-147">保存して、カスタムのデータへのアクセスに関連するほとんどのシナリオで推奨されるソリューションを開いています。</span><span class="sxs-lookup"><span data-stu-id="75308-147">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="75308-148">ただし、 [Microsoft グラフ API メタデータ](https://developer.microsoft.com/graph/docs/overview/call_api)を通じて公開されていない Outlook MAPI プロパティのカスタムのデータにアクセスする必要がある場合は、[拡張プロパティおよびその他の API](extended-properties-overview.md)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="75308-148">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="75308-149">メタデータを公開するプロパティを確認することができます[https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)。</span><span class="sxs-lookup"><span data-stu-id="75308-149">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="75308-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75308-150">JSON representation</span></span>

<span data-ttu-id="75308-151">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="75308-151">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.opentypeextension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a><span data-ttu-id="75308-152">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75308-152">Properties</span></span>

| <span data-ttu-id="75308-153">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75308-153">Property</span></span> | <span data-ttu-id="75308-154">型</span><span class="sxs-lookup"><span data-stu-id="75308-154">Type</span></span> | <span data-ttu-id="75308-155">説明</span><span class="sxs-lookup"><span data-stu-id="75308-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="75308-156">extensionName</span><span class="sxs-lookup"><span data-stu-id="75308-156">extensionName</span></span>|<span data-ttu-id="75308-157">String</span><span class="sxs-lookup"><span data-stu-id="75308-157">String</span></span>|<span data-ttu-id="75308-p106">オープン型のデータ拡張情報の一意のテキスト識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="75308-p106">A unique text identifier for an open type data extension. Required.</span></span>|
|<span data-ttu-id="75308-160">id</span><span class="sxs-lookup"><span data-stu-id="75308-160">id</span></span>|<span data-ttu-id="75308-161">String</span><span class="sxs-lookup"><span data-stu-id="75308-161">String</span></span>| <span data-ttu-id="75308-p107">**extensionName** と拡張子タイプを連結する完全修飾識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="75308-p107">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75308-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="75308-164">Relationships</span></span>

<span data-ttu-id="75308-165">なし</span><span class="sxs-lookup"><span data-stu-id="75308-165">None</span></span>

## <a name="methods"></a><span data-ttu-id="75308-166">メソッド</span><span class="sxs-lookup"><span data-stu-id="75308-166">Methods</span></span>

| <span data-ttu-id="75308-167">メソッド</span><span class="sxs-lookup"><span data-stu-id="75308-167">Method</span></span> | <span data-ttu-id="75308-168">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="75308-168">Return Type</span></span> | <span data-ttu-id="75308-169">説明</span><span class="sxs-lookup"><span data-stu-id="75308-169">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="75308-170">Post</span><span class="sxs-lookup"><span data-stu-id="75308-170">Post</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="75308-171">[openTypeExtension](opentypeextension.md)(既存リソースのインスタンスで)、または、[連絡先](../resources/contact.md)の新しい、[イベント](../resources/event.md)、または openTypeExtension オブジェクトを含む[メッセージ](../resources/message.md)です。</span><span class="sxs-lookup"><span data-stu-id="75308-171">[openTypeExtension](opentypeextension.md)(in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="75308-172">既存または新規のリソース インスタンス内に openTypeExtension オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="75308-172">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="75308-173">Get</span><span class="sxs-lookup"><span data-stu-id="75308-173">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="75308-174">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="75308-174">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="75308-175">openTypeExtension オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="75308-175">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="75308-176">更新する</span><span class="sxs-lookup"><span data-stu-id="75308-176">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="75308-177">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="75308-177">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="75308-178">openTypeExtension オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="75308-178">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="75308-179">削除</span><span class="sxs-lookup"><span data-stu-id="75308-179">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="75308-180">なし</span><span class="sxs-lookup"><span data-stu-id="75308-180">None</span></span> |<span data-ttu-id="75308-181">openTypeExtension オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="75308-181">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/opentypeextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
