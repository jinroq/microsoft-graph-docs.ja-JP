# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="919ad-101">openTypeExtension リソース タイプ (オープン拡張機能)</span><span class="sxs-lookup"><span data-stu-id="919ad-101">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="919ad-102">オープン拡張機能 (旧称は Office 365 のデータ拡張機能) を使用すると、型指定されていないプロパティを Microsoft Graph のリソースに簡単に直接追加できます。</span><span class="sxs-lookup"><span data-stu-id="919ad-102">Open extensions (formerly known as Office 365 data extensions) give you an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span> 

<span data-ttu-id="919ad-103">オープン拡張機能は、**openTypeExtension** リソースで表されます。</span><span class="sxs-lookup"><span data-stu-id="919ad-103">Office 365 data extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="919ad-104">リソースに追加されるオープン拡張機能は **extensions** ナビゲーション プロパティに表示されます。このプロパティは、[extension](extension.md) 抽象型から派生します。</span><span class="sxs-lookup"><span data-stu-id="919ad-104">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span> <span data-ttu-id="919ad-105">各拡張機能には **extensionName** プロパティがあります。このプロパティは、すべての拡張機能とカスタム データで唯一定義済みの書き込み可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="919ad-105">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> 

<span data-ttu-id="919ad-106">拡張機能名が必ず一意であるようにする方法の 1 つは、_独自のドメイン_に依存する逆引きドメイン ネーム システム (DNS) 形式 (例: `Com.Contoso.ContactInfo`) を使用することです。</span><span class="sxs-lookup"><span data-stu-id="919ad-106">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) method that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="919ad-107">拡張機能名に Microsoft ドメイン (`Com.Microsoft` または `Com.OnMicrosoft`) を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="919ad-107">Do not use the Microsoft domain in an extension name.</span></span>

<span data-ttu-id="919ad-108">オープン拡張機能の例:[オープン拡張機能を使用してカスタム データをユーザーに追加する](../../../concepts/extensibility_open_users.md)</span><span class="sxs-lookup"><span data-stu-id="919ad-108">Open extension example: [Add custom data to users using open extensions](../../../concepts/extensibility_open_users.md)</span></span>

<span data-ttu-id="919ad-109">オープン拡張機能は、次のリソースの対応するバージョンの一般提供 (GA: /v1.0 および /ベータ) またはプレビュー (/ベータ) でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="919ad-109">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

|<span data-ttu-id="919ad-110">リソース</span><span class="sxs-lookup"><span data-stu-id="919ad-110">Resource</span></span> |<span data-ttu-id="919ad-111">バージョン</span><span class="sxs-lookup"><span data-stu-id="919ad-111">Version</span></span> |
|:---------------|:-------|
| [<span data-ttu-id="919ad-112">管理単位</span><span class="sxs-lookup"><span data-stu-id="919ad-112">Administrative unit</span></span>](../../beta/resources/administrativeunit.md)  | <span data-ttu-id="919ad-113">プレビューのみ</span><span class="sxs-lookup"><span data-stu-id="919ad-113">Preview only</span></span> |
| [<span data-ttu-id="919ad-114">予定表イベント</span><span class="sxs-lookup"><span data-stu-id="919ad-114">Calendar event</span></span>](event.md) | <span data-ttu-id="919ad-115">GA</span><span class="sxs-lookup"><span data-stu-id="919ad-115">GA</span></span> |
| <span data-ttu-id="919ad-116">グループ[予定表イベント](event.md)</span><span class="sxs-lookup"><span data-stu-id="919ad-116">Group [calendar event](event.md)</span></span> | <span data-ttu-id="919ad-117">GA</span><span class="sxs-lookup"><span data-stu-id="919ad-117">GA</span></span> |
| <span data-ttu-id="919ad-118">グループ会話スレッド[投稿](post.md)</span><span class="sxs-lookup"><span data-stu-id="919ad-118">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="919ad-119">GA</span><span class="sxs-lookup"><span data-stu-id="919ad-119">GA</span></span> |
| [<span data-ttu-id="919ad-120">device</span><span class="sxs-lookup"><span data-stu-id="919ad-120">device</span></span>](device.md) | <span data-ttu-id="919ad-121">GA</span><span class="sxs-lookup"><span data-stu-id="919ad-121">GA</span></span> |
| [<span data-ttu-id="919ad-122">グループ</span><span class="sxs-lookup"><span data-stu-id="919ad-122">group</span></span>](group.md) | <span data-ttu-id="919ad-123">GA</span><span class="sxs-lookup"><span data-stu-id="919ad-123">GA</span></span> |
| [<span data-ttu-id="919ad-124">メッセージ</span><span class="sxs-lookup"><span data-stu-id="919ad-124">message</span></span>](message.md) | <span data-ttu-id="919ad-125">GA</span><span class="sxs-lookup"><span data-stu-id="919ad-125">GA</span></span> |
| [<span data-ttu-id="919ad-126">組織</span><span class="sxs-lookup"><span data-stu-id="919ad-126">organization</span></span>](organization.md) | <span data-ttu-id="919ad-127">GA</span><span class="sxs-lookup"><span data-stu-id="919ad-127">GA</span></span> |
| [<span data-ttu-id="919ad-128">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="919ad-128">Personal contact</span></span>](contact.md) | <span data-ttu-id="919ad-129">GA</span><span class="sxs-lookup"><span data-stu-id="919ad-129">GA</span></span> |
| [<span data-ttu-id="919ad-130">ユーザー</span><span class="sxs-lookup"><span data-stu-id="919ad-130">user</span></span>](user.md) | <span data-ttu-id="919ad-131">GA</span><span class="sxs-lookup"><span data-stu-id="919ad-131">GA</span></span> |

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="919ad-132">オープン拡張機能 (Outlook リソース用) と拡張プロパティのどちらを使用するか</span><span class="sxs-lookup"><span data-stu-id="919ad-132">Use open extensions (for Outlook resources) or extended properties?</span></span>

<span data-ttu-id="919ad-p103">オープン拡張機能は、カスタム データの格納およびカスタムデータへのアクセスを必要とするほとんどのシナリオに対して推奨されるソリューションです。ただし、[拡張プロパティとこの REST API](extended-properties-overview.md) は、[Microsoft Graph API のメタデータ](http://developer.microsoft.com/en-us/graph/docs/overview/call_api)を通じてまだ公開されていない Outlook MAPI プロパティのカスタム データにアクセスする必要がある場合に使用できます。メタデータが公開するプロパティは、https://graph.microsoft.com/v1.0/$metadata で確認できます。</span><span class="sxs-lookup"><span data-stu-id="919ad-p103">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data. If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](http://developer.microsoft.com/en-us/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md). You can verify which properties the metadata exposes at https://graph.microsoft.com/v1.0/$metadata.</span></span>


## <a name="json-representation"></a><span data-ttu-id="919ad-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="919ad-136">JSON representation</span></span>

<span data-ttu-id="919ad-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="919ad-137">Here is a JSON representation of the resource.</span></span>

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

<br/>

## <a name="properties"></a><span data-ttu-id="919ad-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="919ad-138">Properties</span></span>

|<span data-ttu-id="919ad-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="919ad-139">Property</span></span>      |<span data-ttu-id="919ad-140">型</span><span class="sxs-lookup"><span data-stu-id="919ad-140">Type</span></span>    |<span data-ttu-id="919ad-141">説明</span><span class="sxs-lookup"><span data-stu-id="919ad-141">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="919ad-142">extensionName</span><span class="sxs-lookup"><span data-stu-id="919ad-142">extensionName</span></span>|<span data-ttu-id="919ad-143">String</span><span class="sxs-lookup"><span data-stu-id="919ad-143">String</span></span>|<span data-ttu-id="919ad-p104">オープン型のオープン拡張機能の一意のテキスト識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="919ad-p104">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="919ad-146">id</span><span class="sxs-lookup"><span data-stu-id="919ad-146">id</span></span>|<span data-ttu-id="919ad-147">String</span><span class="sxs-lookup"><span data-stu-id="919ad-147">String</span></span>| <span data-ttu-id="919ad-p105">**extensionName** と拡張子タイプを連結する完全修飾識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="919ad-p105">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="919ad-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="919ad-150">Relationships</span></span>

<span data-ttu-id="919ad-151">なし</span><span class="sxs-lookup"><span data-stu-id="919ad-151">None</span></span>


## <a name="methods"></a><span data-ttu-id="919ad-152">メソッド</span><span class="sxs-lookup"><span data-stu-id="919ad-152">Methods</span></span>

|<span data-ttu-id="919ad-153">メソッド</span><span class="sxs-lookup"><span data-stu-id="919ad-153">Method</span></span>        |<span data-ttu-id="919ad-154">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="919ad-154">Return Type</span></span> |<span data-ttu-id="919ad-155">説明</span><span class="sxs-lookup"><span data-stu-id="919ad-155">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="919ad-156">Post</span><span class="sxs-lookup"><span data-stu-id="919ad-156">Post</span></span>](../api/opentypeextension_post_opentypeextension.md) | <span data-ttu-id="919ad-157">(既存リソースのインスタンス内の) [openTypeExtension](opentypeextension.md)、または、openTypeExtension オブジェクトを含む新しい[contact](../resources/contact.md)、[event](../resources/event.md)、[message](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="919ad-157">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="919ad-158">既存または新規のリソース インスタンス内に openTypeExtension オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="919ad-158">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="919ad-159">Get</span><span class="sxs-lookup"><span data-stu-id="919ad-159">Get</span></span>](../api/opentypeextension_get.md) | [<span data-ttu-id="919ad-160">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="919ad-160">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="919ad-161">openTypeExtension オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="919ad-161">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="919ad-162">更新する</span><span class="sxs-lookup"><span data-stu-id="919ad-162">Update</span></span>](../api/opentypeextension_update.md) | [<span data-ttu-id="919ad-163">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="919ad-163">openTypeExtension</span></span>](opentypeextension.md)   |<span data-ttu-id="919ad-164">openTypeExtension オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="919ad-164">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="919ad-165">削除</span><span class="sxs-lookup"><span data-stu-id="919ad-165">Delete</span></span>](../api/opentypeextension_delete.md) | <span data-ttu-id="919ad-166">なし</span><span class="sxs-lookup"><span data-stu-id="919ad-166">None</span></span> |<span data-ttu-id="919ad-167">openTypeExtension オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="919ad-167">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
