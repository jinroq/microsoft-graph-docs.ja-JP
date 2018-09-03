# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="145e4-101">openTypeExtension リソース タイプ (オープン拡張機能)</span><span class="sxs-lookup"><span data-stu-id="145e4-101">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="145e4-102">オープン拡張機能 (旧称は Office 365 のデータ拡張機能) を使用すると、型指定されていないプロパティを Microsoft Graph のリソースに簡単に直接追加できます。</span><span class="sxs-lookup"><span data-stu-id="145e4-102">Open extensions (formerly known as Office 365 data extensions) give you an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>

<span data-ttu-id="145e4-103">オープン拡張機能は、**openTypeExtension** リソースで表されます。</span><span class="sxs-lookup"><span data-stu-id="145e4-103">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="145e4-104">リソースに追加されるオープン拡張機能は **extensions** ナビゲーション プロパティに表示されます。このプロパティは、[extension](extension.md) 抽象型から派生します。</span><span class="sxs-lookup"><span data-stu-id="145e4-104">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span> <span data-ttu-id="145e4-105">各拡張機能には **extensionName** プロパティがあります。このプロパティは、すべての拡張機能とカスタム データで唯一定義済みの書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="145e4-105">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span>

<span data-ttu-id="145e4-106">拡張機能名が必ず一意であるようにする方法の 1 つは、_独自のドメイン_に依存する逆引きドメイン ネーム システム (DNS) 形式 (例: `Com.Contoso.ContactInfo`) を使用することです。</span><span class="sxs-lookup"><span data-stu-id="145e4-106">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="145e4-107">拡張機能名に Microsoft ドメイン (`Com.Microsoft` または `Com.OnMicrosoft`) を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="145e4-107">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="145e4-108">オープン拡張機能の例:[オープン拡張機能を使用してカスタム データをユーザーに追加する](../../../concepts/extensibility_open_users.md)</span><span class="sxs-lookup"><span data-stu-id="145e4-108">Open extension example: [Add custom data to users using open extensions](../../../concepts/extensibility_open_users.md)</span></span>

<span data-ttu-id="145e4-109">オープン拡張機能は、次のリソースの対応するバージョンの一般提供 (GA: /v1.0 および /ベータ) またはプレビュー (/ベータ) でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="145e4-109">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

|<span data-ttu-id="145e4-110">リソース</span><span class="sxs-lookup"><span data-stu-id="145e4-110">Resource</span></span> |<span data-ttu-id="145e4-111">バージョン</span><span class="sxs-lookup"><span data-stu-id="145e4-111">Version</span></span> |
|:---------------|:-------|
| [<span data-ttu-id="145e4-112">管理単位</span><span class="sxs-lookup"><span data-stu-id="145e4-112">Administrative unit</span></span>](../../beta/resources/administrativeunit.md)  | <span data-ttu-id="145e4-113">プレビューのみ</span><span class="sxs-lookup"><span data-stu-id="145e4-113">Preview only</span></span> |
| [<span data-ttu-id="145e4-114">予定表イベント</span><span class="sxs-lookup"><span data-stu-id="145e4-114">Calendar event</span></span>](event.md) | <span data-ttu-id="145e4-115">GA</span><span class="sxs-lookup"><span data-stu-id="145e4-115">GA</span></span> |
| <span data-ttu-id="145e4-116">グループ[予定表イベント](event.md)</span><span class="sxs-lookup"><span data-stu-id="145e4-116">Group [calendar event](event.md)</span></span> | <span data-ttu-id="145e4-117">GA</span><span class="sxs-lookup"><span data-stu-id="145e4-117">GA</span></span> |
| <span data-ttu-id="145e4-118">グループ会話スレッド[投稿](post.md)</span><span class="sxs-lookup"><span data-stu-id="145e4-118">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="145e4-119">GA</span><span class="sxs-lookup"><span data-stu-id="145e4-119">GA</span></span> |
| [<span data-ttu-id="145e4-120">device</span><span class="sxs-lookup"><span data-stu-id="145e4-120">device</span></span>](device.md) | <span data-ttu-id="145e4-121">GA</span><span class="sxs-lookup"><span data-stu-id="145e4-121">GA</span></span> |
| [<span data-ttu-id="145e4-122">グループ</span><span class="sxs-lookup"><span data-stu-id="145e4-122">group</span></span>](group.md) | <span data-ttu-id="145e4-123">GA</span><span class="sxs-lookup"><span data-stu-id="145e4-123">GA</span></span> |
| [<span data-ttu-id="145e4-124">メッセージ</span><span class="sxs-lookup"><span data-stu-id="145e4-124">message</span></span>](message.md) | <span data-ttu-id="145e4-125">GA</span><span class="sxs-lookup"><span data-stu-id="145e4-125">GA</span></span> |
| [<span data-ttu-id="145e4-126">組織</span><span class="sxs-lookup"><span data-stu-id="145e4-126">organization</span></span>](organization.md) | <span data-ttu-id="145e4-127">GA</span><span class="sxs-lookup"><span data-stu-id="145e4-127">GA</span></span> |
| [<span data-ttu-id="145e4-128">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="145e4-128">Personal contact</span></span>](contact.md) | <span data-ttu-id="145e4-129">GA</span><span class="sxs-lookup"><span data-stu-id="145e4-129">GA</span></span> |
| [<span data-ttu-id="145e4-130">ユーザー</span><span class="sxs-lookup"><span data-stu-id="145e4-130">user</span></span>](user.md) | <span data-ttu-id="145e4-131">GA</span><span class="sxs-lookup"><span data-stu-id="145e4-131">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="145e4-132">Outlook に固有の考慮事項</span><span class="sxs-lookup"><span data-stu-id="145e4-132">Outlook-specific considerations</span></span>

<span data-ttu-id="145e4-133">Outlook のリソース上に存在する各オープン拡張 (イベント、メッセージ、または個人用の連絡先) は、[MAPI の名前付きプロパティ](https://msdn.microsoft.com/en-us/library/cc765864(v=office.15).aspx) に格納されます。</span><span class="sxs-lookup"><span data-stu-id="145e4-133">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/en-us/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="145e4-134">Outlook でオープン拡張を作成する際には、MAPI の名前付きプロパティを、ユーザーのメールボックス内の有限のリソースとみなします。</span><span class="sxs-lookup"><span data-stu-id="145e4-134">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="145e4-135">ユーザーの名前付きプロパティのクォータが不足すると、そのユーザーに対しそれ以上の名前付きプロパティを作成できません。</span><span class="sxs-lookup"><span data-stu-id="145e4-135">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="145e4-136">その場合、機能する名前付きプロパティに依存するクライアントで予期しない動作が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="145e4-136">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="145e4-137">Outlook のリソースでオープン拡張を作製する場合には、次のガイドラインを適用します。</span><span class="sxs-lookup"><span data-stu-id="145e4-137">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="145e4-138">必要な最小数の拡張機能を作成します。</span><span class="sxs-lookup"><span data-stu-id="145e4-138">Create the minimum number of extensions required.</span></span> <span data-ttu-id="145e4-139">ほとんどのアプリケーションでは、複数の拡張機能が必要です。</span><span class="sxs-lookup"><span data-stu-id="145e4-139">Most applications should require no more than one extension.</span></span> <span data-ttu-id="145e4-140">拡張機能には定義されたプロパティや構造がないため、単一の拡張機能に複数の値を格納することができます。</span><span class="sxs-lookup"><span data-stu-id="145e4-140">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="145e4-141">(ユーザー入力などに基づく) 変数の方法で拡張機能の名前付けをしないでください。</span><span class="sxs-lookup"><span data-stu-id="145e4-141">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="145e4-142">ユーザーのメールボックスで以前に使用されたことがない新しい名前でオープン拡張が作成されるたびに、新しい MAPI 名前付きプロパティが作成されます。</span><span class="sxs-lookup"><span data-stu-id="145e4-142">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="145e4-143">拡張子を削除しても、名前付きプロパティは削除されません。</span><span class="sxs-lookup"><span data-stu-id="145e4-143">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="145e4-144">オープン拡張 (Outlook リソース用) または拡張プロパティを使用</span><span class="sxs-lookup"><span data-stu-id="145e4-144">Use open extensions (for Outlook resources) or extended properties?</span></span>

<span data-ttu-id="145e4-145">オープン拡張は、カスタム データの格納およびカスタムデータへのアクセスを必要とするほとんどのシナリオで推奨されるソリューションです。</span><span class="sxs-lookup"><span data-stu-id="145e4-145">Data extensions is the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="145e4-146">ただし、[Microsoft Graph API メタデータ](http://developer.microsoft.com/en-us/graph/docs/overview/call_api) を通じてすでに公開されていない Outlook MAPI プロパティのカスタム データにアクセスする必要がある場合は、[拡張プロパティとその REST API](extended-properties-overview.md) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="145e4-146">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the Outlook REST API metadata, you can use extended properties and its REST API.</span></span> <span data-ttu-id="145e4-147">メタデータがどのプロパティを公開するかは [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata) で確認できます。</span><span class="sxs-lookup"><span data-stu-id="145e4-147">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="145e4-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="145e4-148">JSON representation</span></span>

<span data-ttu-id="145e4-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="145e4-149">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="145e4-150">プロパティ</span><span class="sxs-lookup"><span data-stu-id="145e4-150">Properties</span></span>

|<span data-ttu-id="145e4-151">プロパティ</span><span class="sxs-lookup"><span data-stu-id="145e4-151">Property</span></span> | <span data-ttu-id="145e4-152">タイプ</span><span class="sxs-lookup"><span data-stu-id="145e4-152">Type</span></span> | <span data-ttu-id="145e4-153">説明</span><span class="sxs-lookup"><span data-stu-id="145e4-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="145e4-154">extensionName</span><span class="sxs-lookup"><span data-stu-id="145e4-154">extensionName</span></span>|<span data-ttu-id="145e4-155">文字列</span><span class="sxs-lookup"><span data-stu-id="145e4-155">String</span></span>|<span data-ttu-id="145e4-p107">オープン型のオープン拡張機能の一意のテキスト識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="145e4-p107">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="145e4-158">id</span><span class="sxs-lookup"><span data-stu-id="145e4-158">id</span></span>|<span data-ttu-id="145e4-159">文字列</span><span class="sxs-lookup"><span data-stu-id="145e4-159">String</span></span>| <span data-ttu-id="145e4-p108">**extensionName** と拡張子タイプを連結する完全修飾識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="145e4-p108">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="145e4-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="145e4-162">Relationships</span></span>

<span data-ttu-id="145e4-163">なし</span><span class="sxs-lookup"><span data-stu-id="145e4-163">None</span></span>

## <a name="methods"></a><span data-ttu-id="145e4-164">メソッド</span><span class="sxs-lookup"><span data-stu-id="145e4-164">Methods</span></span>

|<span data-ttu-id="145e4-165">メソッド</span><span class="sxs-lookup"><span data-stu-id="145e4-165">Method</span></span> | <span data-ttu-id="145e4-166">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="145e4-166">Return Type</span></span> | <span data-ttu-id="145e4-167">説明</span><span class="sxs-lookup"><span data-stu-id="145e4-167">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="145e4-168">投稿</span><span class="sxs-lookup"><span data-stu-id="145e4-168">Post</span></span>](../api/opentypeextension_post_opentypeextension.md) | <span data-ttu-id="145e4-169">(既存リソースのインスタンス内の) [openTypeExtension](opentypeextension.md)、または、openTypeExtension オブジェクトを含む新しい[contact](../resources/contact.md)、[event](../resources/event.md)、[message](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="145e4-169">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object</span></span> | <span data-ttu-id="145e4-170">既存または新規のリソース インスタンス内に openTypeExtension オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="145e4-170">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="145e4-171">取得</span><span class="sxs-lookup"><span data-stu-id="145e4-171">Get</span></span>](../api/opentypeextension_get.md) | [<span data-ttu-id="145e4-172">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="145e4-172">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="145e4-173">openTypeExtension オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="145e4-173">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="145e4-174">更新する</span><span class="sxs-lookup"><span data-stu-id="145e4-174">Update</span></span>](../api/opentypeextension_update.md) | [<span data-ttu-id="145e4-175">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="145e4-175">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="145e4-176">openTypeExtension オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="145e4-176">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="145e4-177">削除</span><span class="sxs-lookup"><span data-stu-id="145e4-177">Delete</span></span>](../api/opentypeextension_delete.md) | <span data-ttu-id="145e4-178">なし</span><span class="sxs-lookup"><span data-stu-id="145e4-178">None</span></span> |<span data-ttu-id="145e4-179">openTypeExtension オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="145e4-179">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
