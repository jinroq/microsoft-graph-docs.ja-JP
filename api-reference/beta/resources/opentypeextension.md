---
title: openTypeExtension リソース タイプ (オープン拡張機能)
description: (Office 365 のデータ拡張機能と呼ばれていました) 開いているの拡張機能では、直接グラフ内のリソースに型指定されていないプロパティを追加する簡単な方法を提供します。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 323d44c839a9df5e9103311f50d239ba34fbb348
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923916"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="b531e-103">openTypeExtension リソース タイプ (オープン拡張機能)</span><span class="sxs-lookup"><span data-stu-id="b531e-103">openTypeExtension resource type (open extensions)</span></span>

> <span data-ttu-id="b531e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b531e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b531e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b531e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b531e-106">(Office 365 のデータ拡張機能と呼ばれていました) 開いているの拡張機能では、直接グラフ内のリソースに型指定されていないプロパティを追加する簡単な方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="b531e-106">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>
<span data-ttu-id="b531e-107">オープン拡張機能は、**openTypeExtension** リソースで表されます。</span><span class="sxs-lookup"><span data-stu-id="b531e-107">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="b531e-108">リソースに追加されるオープン拡張機能は **extensions** ナビゲーション プロパティに表示されます。このプロパティは、[extension](extension.md) 抽象型から派生します。</span><span class="sxs-lookup"><span data-stu-id="b531e-108">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span>  <span data-ttu-id="b531e-109">各拡張機能には **extensionName** プロパティがあります。このプロパティは、すべての拡張機能とカスタム データで唯一定義済みの書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="b531e-109">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> <span data-ttu-id="b531e-110">拡張機能名が必ず一意であるようにする方法の 1 つは、_独自のドメイン_に依存する逆引きドメイン ネーム システム (DNS) 形式 (例: `Com.Contoso.ContactInfo`) を使用することです。</span><span class="sxs-lookup"><span data-stu-id="b531e-110">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="b531e-111">拡張機能名に Microsoft ドメイン (`Com.Microsoft` または `Com.OnMicrosoft`) を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="b531e-111">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="b531e-112">オープン拡張機能の例:[オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="b531e-112">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="b531e-113">オープン拡張機能は、次のリソースの対応するバージョンの一般提供 (GA: /v1.0 および /ベータ) またはプレビュー (/ベータ) でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b531e-113">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="b531e-114">リソース</span><span class="sxs-lookup"><span data-stu-id="b531e-114">Resource</span></span> | <span data-ttu-id="b531e-115">バージョン</span><span class="sxs-lookup"><span data-stu-id="b531e-115">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="b531e-116">管理単位</span><span class="sxs-lookup"><span data-stu-id="b531e-116">Administrative unit</span></span>](administrativeunit.md)  | <span data-ttu-id="b531e-117">プレビューのみ</span><span class="sxs-lookup"><span data-stu-id="b531e-117">Preview only</span></span> |
| [<span data-ttu-id="b531e-118">予定表イベント</span><span class="sxs-lookup"><span data-stu-id="b531e-118">Calendar event</span></span>](event.md) | <span data-ttu-id="b531e-119">GA</span><span class="sxs-lookup"><span data-stu-id="b531e-119">GA</span></span> |
| <span data-ttu-id="b531e-120">グループ[予定表イベント](event.md)</span><span class="sxs-lookup"><span data-stu-id="b531e-120">Group [calendar event](event.md)</span></span> | <span data-ttu-id="b531e-121">GA</span><span class="sxs-lookup"><span data-stu-id="b531e-121">GA</span></span> |
| <span data-ttu-id="b531e-122">グループ会話スレッド[投稿](post.md)</span><span class="sxs-lookup"><span data-stu-id="b531e-122">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="b531e-123">GA</span><span class="sxs-lookup"><span data-stu-id="b531e-123">GA</span></span> |
| [<span data-ttu-id="b531e-124">device</span><span class="sxs-lookup"><span data-stu-id="b531e-124">device</span></span>](device.md) | <span data-ttu-id="b531e-125">GA</span><span class="sxs-lookup"><span data-stu-id="b531e-125">GA</span></span> |
| [<span data-ttu-id="b531e-126">グループ</span><span class="sxs-lookup"><span data-stu-id="b531e-126">group</span></span>](group.md) | <span data-ttu-id="b531e-127">GA</span><span class="sxs-lookup"><span data-stu-id="b531e-127">GA</span></span> |
| [<span data-ttu-id="b531e-128">メッセージ</span><span class="sxs-lookup"><span data-stu-id="b531e-128">message</span></span>](message.md) | <span data-ttu-id="b531e-129">GA</span><span class="sxs-lookup"><span data-stu-id="b531e-129">GA</span></span> |
| [<span data-ttu-id="b531e-130">組織</span><span class="sxs-lookup"><span data-stu-id="b531e-130">organization</span></span>](organization.md) | <span data-ttu-id="b531e-131">GA</span><span class="sxs-lookup"><span data-stu-id="b531e-131">GA</span></span> |
| [<span data-ttu-id="b531e-132">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="b531e-132">Personal contact</span></span>](contact.md) | <span data-ttu-id="b531e-133">GA</span><span class="sxs-lookup"><span data-stu-id="b531e-133">GA</span></span> |
| [<span data-ttu-id="b531e-134">ユーザー</span><span class="sxs-lookup"><span data-stu-id="b531e-134">user</span></span>](user.md) | <span data-ttu-id="b531e-135">GA</span><span class="sxs-lookup"><span data-stu-id="b531e-135">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="b531e-136">Outlook に固有の考慮事項</span><span class="sxs-lookup"><span data-stu-id="b531e-136">Outlook-specific considerations</span></span>

<span data-ttu-id="b531e-137">(イベント、メッセージ、または個人用の連絡先)、Outlook のリソース上に存在の開いている各拡張機能は、 [MAPI の名前付きプロパティ](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)に格納されます。</span><span class="sxs-lookup"><span data-stu-id="b531e-137">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="b531e-138">Outlook を開いている拡張機能を作成するときは、MAPI プロパティを名前付きのユーザーのメールボックス内の有限のリソースであることを検討します。</span><span class="sxs-lookup"><span data-stu-id="b531e-138">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="b531e-139">ユーザーの名前付きプロパティのクォータが不足すると、そのユーザーに対して複数の名前付きプロパティを作成できません。</span><span class="sxs-lookup"><span data-stu-id="b531e-139">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="b531e-140">その場合、関数の名前付きプロパティに依存するクライアントからの予期しない動作します。</span><span class="sxs-lookup"><span data-stu-id="b531e-140">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="b531e-141">Outlook のリソースで開いている拡張機能を作成するときは、次のガイドラインを適用します。</span><span class="sxs-lookup"><span data-stu-id="b531e-141">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="b531e-142">必要な拡張の最小数を作成します。</span><span class="sxs-lookup"><span data-stu-id="b531e-142">Create the minimum number of extensions required.</span></span> <span data-ttu-id="b531e-143">ほとんどのアプリケーションは、複数の拡張機能を必要があります。</span><span class="sxs-lookup"><span data-stu-id="b531e-143">Most applications should require no more than one extension.</span></span> <span data-ttu-id="b531e-144">拡張機能があるないプロパティの設定を定義または構造体は、単一の拡張機能に複数の値を格納することができますので。</span><span class="sxs-lookup"><span data-stu-id="b531e-144">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="b531e-145">(などのユーザー入力などに基づきます)。 変数の方法で拡張機能の名前付けをしないでください。</span><span class="sxs-lookup"><span data-stu-id="b531e-145">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="b531e-146">前に、ユーザーのメールボックスで使用されていない新しい名前で開いている拡張機能を作成するたびに、新しい MAPI 名前付きプロパティが作成されます。</span><span class="sxs-lookup"><span data-stu-id="b531e-146">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="b531e-147">拡張子を削除しても、名前付きプロパティは削除されません。</span><span class="sxs-lookup"><span data-stu-id="b531e-147">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="b531e-148">(Outlook のリソース) の拡張子を開くか、拡張プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="b531e-148">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="b531e-149">保存して、カスタムのデータへのアクセスに関連するほとんどのシナリオで推奨されるソリューションを開いています。</span><span class="sxs-lookup"><span data-stu-id="b531e-149">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="b531e-150">ただし、 [Microsoft グラフ API メタデータ](https://developer.microsoft.com/graph/docs/overview/call_api)を通じて公開されていない Outlook MAPI プロパティのカスタムのデータにアクセスする必要がある場合は、[拡張プロパティおよびその他の API](extended-properties-overview.md)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="b531e-150">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="b531e-151">メタデータを公開するプロパティを確認することができます[https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)。</span><span class="sxs-lookup"><span data-stu-id="b531e-151">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b531e-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b531e-152">JSON representation</span></span>

<span data-ttu-id="b531e-153">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b531e-153">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="b531e-154">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b531e-154">Properties</span></span>

| <span data-ttu-id="b531e-155">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b531e-155">Property</span></span> | <span data-ttu-id="b531e-156">型</span><span class="sxs-lookup"><span data-stu-id="b531e-156">Type</span></span> | <span data-ttu-id="b531e-157">説明</span><span class="sxs-lookup"><span data-stu-id="b531e-157">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b531e-158">extensionName</span><span class="sxs-lookup"><span data-stu-id="b531e-158">extensionName</span></span>|<span data-ttu-id="b531e-159">String</span><span class="sxs-lookup"><span data-stu-id="b531e-159">String</span></span>|<span data-ttu-id="b531e-p107">オープン型のデータ拡張情報の一意のテキスト識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="b531e-p107">A unique text identifier for an open type data extension. Required.</span></span>|
|<span data-ttu-id="b531e-162">id</span><span class="sxs-lookup"><span data-stu-id="b531e-162">id</span></span>|<span data-ttu-id="b531e-163">String</span><span class="sxs-lookup"><span data-stu-id="b531e-163">String</span></span>| <span data-ttu-id="b531e-p108">**extensionName** と拡張子タイプを連結する完全修飾識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b531e-p108">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b531e-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b531e-166">Relationships</span></span>

<span data-ttu-id="b531e-167">なし</span><span class="sxs-lookup"><span data-stu-id="b531e-167">None</span></span>

## <a name="methods"></a><span data-ttu-id="b531e-168">メソッド</span><span class="sxs-lookup"><span data-stu-id="b531e-168">Methods</span></span>

| <span data-ttu-id="b531e-169">メソッド</span><span class="sxs-lookup"><span data-stu-id="b531e-169">Method</span></span> | <span data-ttu-id="b531e-170">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b531e-170">Return Type</span></span> | <span data-ttu-id="b531e-171">説明</span><span class="sxs-lookup"><span data-stu-id="b531e-171">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="b531e-172">Post</span><span class="sxs-lookup"><span data-stu-id="b531e-172">Post</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="b531e-173">[openTypeExtension](opentypeextension.md)(既存リソースのインスタンスで)、または、[連絡先](../resources/contact.md)の新しい、[イベント](../resources/event.md)、または openTypeExtension オブジェクトを含む[メッセージ](../resources/message.md)です。</span><span class="sxs-lookup"><span data-stu-id="b531e-173">[openTypeExtension](opentypeextension.md)(in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="b531e-174">既存または新規のリソース インスタンス内に openTypeExtension オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b531e-174">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="b531e-175">Get</span><span class="sxs-lookup"><span data-stu-id="b531e-175">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="b531e-176">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="b531e-176">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="b531e-177">openTypeExtension オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b531e-177">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="b531e-178">更新する</span><span class="sxs-lookup"><span data-stu-id="b531e-178">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="b531e-179">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="b531e-179">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="b531e-180">openTypeExtension オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b531e-180">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="b531e-181">削除</span><span class="sxs-lookup"><span data-stu-id="b531e-181">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="b531e-182">なし</span><span class="sxs-lookup"><span data-stu-id="b531e-182">None</span></span> |<span data-ttu-id="b531e-183">openTypeExtension オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="b531e-183">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
