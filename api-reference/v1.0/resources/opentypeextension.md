# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="68cb8-101">openTypeExtension リソース タイプ (オープン拡張機能)</span><span class="sxs-lookup"><span data-stu-id="68cb8-101">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="68cb8-102">(Office 365 のデータ拡張機能と呼ばれていました) 開いているの拡張機能では、直接グラフ内のリソースに型指定されていないプロパティを追加する簡単な方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="68cb8-102">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>

<span data-ttu-id="68cb8-103">オープン拡張機能は、**openTypeExtension** リソースで表されます。</span><span class="sxs-lookup"><span data-stu-id="68cb8-103">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="68cb8-104">リソースに追加されるオープン拡張機能は **extensions** ナビゲーション プロパティに表示されます。このプロパティは、[extension](extension.md) 抽象型から派生します。</span><span class="sxs-lookup"><span data-stu-id="68cb8-104">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span> <span data-ttu-id="68cb8-105">各拡張機能には **extensionName** プロパティがあります。このプロパティは、すべての拡張機能とカスタム データで唯一定義済みの書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="68cb8-105">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span>

<span data-ttu-id="68cb8-106">拡張機能名が必ず一意であるようにする方法の 1 つは、_独自のドメイン_に依存する逆引きドメイン ネーム システム (DNS) 形式 (例: `Com.Contoso.ContactInfo`) を使用することです。</span><span class="sxs-lookup"><span data-stu-id="68cb8-106">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="68cb8-107">拡張機能名に Microsoft ドメイン (`Com.Microsoft` または `Com.OnMicrosoft`) を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="68cb8-107">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="68cb8-108">オープン拡張機能の例:[オープン拡張機能を使用してカスタム データをユーザーに追加する](../../../concepts/extensibility_open_users.md)</span><span class="sxs-lookup"><span data-stu-id="68cb8-108">Open extension example: [Add custom data to users using open extensions](../../../concepts/extensibility_open_users.md)</span></span>

<span data-ttu-id="68cb8-109">オープン拡張機能は、次のリソースの対応するバージョンの一般提供 (GA: /v1.0 および /ベータ) またはプレビュー (/ベータ) でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="68cb8-109">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

|<span data-ttu-id="68cb8-110">リソース</span><span class="sxs-lookup"><span data-stu-id="68cb8-110">Resource</span></span> |<span data-ttu-id="68cb8-111">バージョン</span><span class="sxs-lookup"><span data-stu-id="68cb8-111">Version</span></span> |
|:---------------|:-------|
| [<span data-ttu-id="68cb8-112">管理単位</span><span class="sxs-lookup"><span data-stu-id="68cb8-112">Administrative unit</span></span>](../../beta/resources/administrativeunit.md)  | <span data-ttu-id="68cb8-113">プレビューのみ</span><span class="sxs-lookup"><span data-stu-id="68cb8-113">Preview only</span></span> |
| [<span data-ttu-id="68cb8-114">予定表イベント</span><span class="sxs-lookup"><span data-stu-id="68cb8-114">Calendar event</span></span>](event.md) | <span data-ttu-id="68cb8-115">GA</span><span class="sxs-lookup"><span data-stu-id="68cb8-115">GA</span></span> |
| <span data-ttu-id="68cb8-116">グループ[予定表イベント](event.md)</span><span class="sxs-lookup"><span data-stu-id="68cb8-116">Group [calendar event](event.md)</span></span> | <span data-ttu-id="68cb8-117">GA</span><span class="sxs-lookup"><span data-stu-id="68cb8-117">GA</span></span> |
| <span data-ttu-id="68cb8-118">グループ会話スレッド[投稿](post.md)</span><span class="sxs-lookup"><span data-stu-id="68cb8-118">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="68cb8-119">GA</span><span class="sxs-lookup"><span data-stu-id="68cb8-119">GA</span></span> |
| [<span data-ttu-id="68cb8-120">device</span><span class="sxs-lookup"><span data-stu-id="68cb8-120">device</span></span>](device.md) | <span data-ttu-id="68cb8-121">GA</span><span class="sxs-lookup"><span data-stu-id="68cb8-121">GA</span></span> |
| [<span data-ttu-id="68cb8-122">グループ</span><span class="sxs-lookup"><span data-stu-id="68cb8-122">group</span></span>](group.md) | <span data-ttu-id="68cb8-123">GA</span><span class="sxs-lookup"><span data-stu-id="68cb8-123">GA</span></span> |
| [<span data-ttu-id="68cb8-124">メッセージ</span><span class="sxs-lookup"><span data-stu-id="68cb8-124">message</span></span>](message.md) | <span data-ttu-id="68cb8-125">GA</span><span class="sxs-lookup"><span data-stu-id="68cb8-125">GA</span></span> |
| [<span data-ttu-id="68cb8-126">組織</span><span class="sxs-lookup"><span data-stu-id="68cb8-126">organization</span></span>](organization.md) | <span data-ttu-id="68cb8-127">GA</span><span class="sxs-lookup"><span data-stu-id="68cb8-127">GA</span></span> |
| [<span data-ttu-id="68cb8-128">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="68cb8-128">Personal contact</span></span>](contact.md) | <span data-ttu-id="68cb8-129">GA</span><span class="sxs-lookup"><span data-stu-id="68cb8-129">GA</span></span> |
| [<span data-ttu-id="68cb8-130">ユーザー</span><span class="sxs-lookup"><span data-stu-id="68cb8-130">user</span></span>](user.md) | <span data-ttu-id="68cb8-131">GA</span><span class="sxs-lookup"><span data-stu-id="68cb8-131">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="68cb8-132">Outlook に固有の考慮事項</span><span class="sxs-lookup"><span data-stu-id="68cb8-132">Outlook-specific considerations</span></span>

<span data-ttu-id="68cb8-133">(イベント、メッセージ、または個人用の連絡先)、Outlook のリソース上に存在の開いている各拡張機能は、 [MAPI の名前付きプロパティ](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)に格納されます。</span><span class="sxs-lookup"><span data-stu-id="68cb8-133">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="68cb8-134">Outlook を開いている拡張機能を作成するときは、MAPI プロパティを名前付きのユーザーのメールボックス内の有限のリソースであることを検討します。</span><span class="sxs-lookup"><span data-stu-id="68cb8-134">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="68cb8-135">ユーザーの名前付きプロパティのクォータが不足すると、そのユーザーに対して複数の名前付きプロパティを作成できません。</span><span class="sxs-lookup"><span data-stu-id="68cb8-135">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="68cb8-136">その場合、関数の名前付きプロパティに依存するクライアントからの予期しない動作します。</span><span class="sxs-lookup"><span data-stu-id="68cb8-136">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="68cb8-137">Outlook のリソースで開いている拡張機能を作成するときは、次のガイドラインを適用します。</span><span class="sxs-lookup"><span data-stu-id="68cb8-137">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="68cb8-138">必要な拡張の最小数を作成します。</span><span class="sxs-lookup"><span data-stu-id="68cb8-138">Create the minimum number of extensions required.</span></span> <span data-ttu-id="68cb8-139">ほとんどのアプリケーションは、複数の拡張機能を必要があります。</span><span class="sxs-lookup"><span data-stu-id="68cb8-139">Most applications should require no more than one extension.</span></span> <span data-ttu-id="68cb8-140">拡張機能があるないプロパティの設定を定義または構造体は、単一の拡張機能に複数の値を格納することができますので。</span><span class="sxs-lookup"><span data-stu-id="68cb8-140">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="68cb8-141">(などのユーザー入力などに基づきます)。 変数の方法で拡張機能の名前付けをしないでください。</span><span class="sxs-lookup"><span data-stu-id="68cb8-141">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="68cb8-142">前に、ユーザーのメールボックスで使用されていない新しい名前で開いている拡張機能を作成するたびに、新しい MAPI 名前付きプロパティが作成されます。</span><span class="sxs-lookup"><span data-stu-id="68cb8-142">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="68cb8-143">拡張子を削除しても、名前付きプロパティは削除されません。</span><span class="sxs-lookup"><span data-stu-id="68cb8-143">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="68cb8-144">(Outlook のリソース) の拡張子を開くか、拡張プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="68cb8-144">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="68cb8-145">開いている拡張機能を保存して、カスタムのデータへのアクセスに関連するほとんどのシナリオで推奨される解決策です。</span><span class="sxs-lookup"><span data-stu-id="68cb8-145">Open extensions are the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="68cb8-146">ただし、 [Microsoft グラフ API メタデータ](https://developer.microsoft.com/graph/docs/overview/call_api)を通じて公開されていない Outlook MAPI プロパティのカスタムのデータにアクセスする必要がある場合は、[拡張プロパティおよびその他の API](extended-properties-overview.md)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="68cb8-146">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="68cb8-147">メタデータを公開するプロパティを確認することができます[https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)。</span><span class="sxs-lookup"><span data-stu-id="68cb8-147">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="68cb8-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68cb8-148">JSON representation</span></span>

<span data-ttu-id="68cb8-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68cb8-149">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="68cb8-150">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68cb8-150">Properties</span></span>

|<span data-ttu-id="68cb8-151">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68cb8-151">Property</span></span> | <span data-ttu-id="68cb8-152">型</span><span class="sxs-lookup"><span data-stu-id="68cb8-152">Type</span></span> | <span data-ttu-id="68cb8-153">説明</span><span class="sxs-lookup"><span data-stu-id="68cb8-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="68cb8-154">extensionName</span><span class="sxs-lookup"><span data-stu-id="68cb8-154">extensionName</span></span>|<span data-ttu-id="68cb8-155">String</span><span class="sxs-lookup"><span data-stu-id="68cb8-155">String</span></span>|<span data-ttu-id="68cb8-p107">オープン型のオープン拡張機能の一意のテキスト識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="68cb8-p107">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="68cb8-158">id</span><span class="sxs-lookup"><span data-stu-id="68cb8-158">id</span></span>|<span data-ttu-id="68cb8-159">文字列</span><span class="sxs-lookup"><span data-stu-id="68cb8-159">String</span></span>| <span data-ttu-id="68cb8-p108">**extensionName** と拡張子タイプを連結する完全修飾識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="68cb8-p108">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68cb8-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="68cb8-162">Relationships</span></span>

<span data-ttu-id="68cb8-163">なし</span><span class="sxs-lookup"><span data-stu-id="68cb8-163">None</span></span>

## <a name="methods"></a><span data-ttu-id="68cb8-164">メソッド</span><span class="sxs-lookup"><span data-stu-id="68cb8-164">Methods</span></span>

|<span data-ttu-id="68cb8-165">メソッド</span><span class="sxs-lookup"><span data-stu-id="68cb8-165">Method</span></span> | <span data-ttu-id="68cb8-166">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="68cb8-166">Return Type</span></span> | <span data-ttu-id="68cb8-167">説明</span><span class="sxs-lookup"><span data-stu-id="68cb8-167">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="68cb8-168">Post</span><span class="sxs-lookup"><span data-stu-id="68cb8-168">Post</span></span>](../api/opentypeextension_post_opentypeextension.md) | <span data-ttu-id="68cb8-169">(既存リソースのインスタンス内の) [openTypeExtension](opentypeextension.md)、または、openTypeExtension オブジェクトを含む新しい[contact](../resources/contact.md)、[event](../resources/event.md)、[message](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="68cb8-169">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object</span></span> | <span data-ttu-id="68cb8-170">既存または新規のリソース インスタンス内に openTypeExtension オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="68cb8-170">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="68cb8-171">Get</span><span class="sxs-lookup"><span data-stu-id="68cb8-171">Get</span></span>](../api/opentypeextension_get.md) | [<span data-ttu-id="68cb8-172">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="68cb8-172">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="68cb8-173">openTypeExtension オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="68cb8-173">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="68cb8-174">更新する</span><span class="sxs-lookup"><span data-stu-id="68cb8-174">Update</span></span>](../api/opentypeextension_update.md) | [<span data-ttu-id="68cb8-175">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="68cb8-175">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="68cb8-176">openTypeExtension オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="68cb8-176">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="68cb8-177">削除</span><span class="sxs-lookup"><span data-stu-id="68cb8-177">Delete</span></span>](../api/opentypeextension_delete.md) | <span data-ttu-id="68cb8-178">なし</span><span class="sxs-lookup"><span data-stu-id="68cb8-178">None</span></span> |<span data-ttu-id="68cb8-179">openTypeExtension オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="68cb8-179">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
