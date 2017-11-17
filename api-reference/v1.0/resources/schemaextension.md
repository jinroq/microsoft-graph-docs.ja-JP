# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="ca72a-101">schemaExtension リソースの種類 (スキーマ拡張機能)</span><span class="sxs-lookup"><span data-stu-id="ca72a-101">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="ca72a-p101">スキーマの拡張機能を使用すると、拡張するスキーマを定義し、厳密に型指定されたカスタム データをリソースの種類に追加できます。カスタム データは拡張したリソースの複合型として表示されます。</span><span class="sxs-lookup"><span data-stu-id="ca72a-p101">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="ca72a-104">スキーマ拡張機能は次のリソースの種類でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="ca72a-104">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="ca72a-105">contact</span><span class="sxs-lookup"><span data-stu-id="ca72a-105">contact</span></span>](contact.md)
 - [<span data-ttu-id="ca72a-106">device</span><span class="sxs-lookup"><span data-stu-id="ca72a-106">device</span></span>](device.md)
 - <span data-ttu-id="ca72a-107">ユーザーまたは Office 365 グループ カレンダーの [event](event.md)</span><span class="sxs-lookup"><span data-stu-id="ca72a-107">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="ca72a-108">Office 365 グループの [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="ca72a-108">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="ca72a-109">group</span><span class="sxs-lookup"><span data-stu-id="ca72a-109">group</span></span>](group.md)
 - [<span data-ttu-id="ca72a-110">message</span><span class="sxs-lookup"><span data-stu-id="ca72a-110">message</span></span>](message.md) 
 - [<span data-ttu-id="ca72a-111">organization</span><span class="sxs-lookup"><span data-stu-id="ca72a-111">organization</span></span>](organization.md)
 - [<span data-ttu-id="ca72a-112">user</span><span class="sxs-lookup"><span data-stu-id="ca72a-112">user</span></span>](user.md)

<span data-ttu-id="ca72a-113">カスタム データのグループへの追加方法については、[スキーマ拡張機能の例](../../../concepts/extensibility_schema_groups.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca72a-113">See the [schema extension example](../../../concepts/extensibility_schema_groups.md) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="ca72a-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="ca72a-114">Methods</span></span>

| <span data-ttu-id="ca72a-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="ca72a-115">Method</span></span>           | <span data-ttu-id="ca72a-116">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ca72a-116">Return Type</span></span>    |<span data-ttu-id="ca72a-117">説明</span><span class="sxs-lookup"><span data-stu-id="ca72a-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ca72a-118">Create</span><span class="sxs-lookup"><span data-stu-id="ca72a-118">Create</span></span>](../api/schemaextension_post_schemaextensions.md) | <span data-ttu-id="ca72a-119">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="ca72a-119">schemaExtension</span></span> |<span data-ttu-id="ca72a-120">スキーマ拡張機能の定義を作成します。</span><span class="sxs-lookup"><span data-stu-id="ca72a-120">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="ca72a-121">List</span><span class="sxs-lookup"><span data-stu-id="ca72a-121">List</span></span>](../api/schemaextension_list.md) | <span data-ttu-id="ca72a-122">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="ca72a-122">schemaExtension</span></span> |<span data-ttu-id="ca72a-123">使用可能な schemaExtension の定義とそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ca72a-123">List the available schemaExtension definitions and their properties.</span></span>|
|[<span data-ttu-id="ca72a-124">Get</span><span class="sxs-lookup"><span data-stu-id="ca72a-124">Get</span></span>](../api/schemaextension_get.md) | <span data-ttu-id="ca72a-125">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="ca72a-125">schemaExtension</span></span> |<span data-ttu-id="ca72a-126">特定の schemaExtension 定義のプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ca72a-126">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="ca72a-127">Update</span><span class="sxs-lookup"><span data-stu-id="ca72a-127">Update</span></span>](../api/schemaextension_update.md) | <span data-ttu-id="ca72a-128">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="ca72a-128">schemaExtension</span></span>   |<span data-ttu-id="ca72a-129">schemaExtension 定義を更新します。</span><span class="sxs-lookup"><span data-stu-id="ca72a-129">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="ca72a-130">Delete</span><span class="sxs-lookup"><span data-stu-id="ca72a-130">Delete</span></span>](../api/schemaextension_delete.md) | <span data-ttu-id="ca72a-131">なし</span><span class="sxs-lookup"><span data-stu-id="ca72a-131">None</span></span> |<span data-ttu-id="ca72a-132">schemaExtension 定義を削除します。</span><span class="sxs-lookup"><span data-stu-id="ca72a-132">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="ca72a-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca72a-133">Properties</span></span>
| <span data-ttu-id="ca72a-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca72a-134">Property</span></span>     | <span data-ttu-id="ca72a-135">型</span><span class="sxs-lookup"><span data-stu-id="ca72a-135">Type</span></span>   |<span data-ttu-id="ca72a-136">説明</span><span class="sxs-lookup"><span data-stu-id="ca72a-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca72a-137">description</span><span class="sxs-lookup"><span data-stu-id="ca72a-137">description</span></span>|<span data-ttu-id="ca72a-138">String</span><span class="sxs-lookup"><span data-stu-id="ca72a-138">String</span></span>|<span data-ttu-id="ca72a-139">スキーマ拡張機能の説明。</span><span class="sxs-lookup"><span data-stu-id="ca72a-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="ca72a-140">id</span><span class="sxs-lookup"><span data-stu-id="ca72a-140">id</span></span>|<span data-ttu-id="ca72a-141">String</span><span class="sxs-lookup"><span data-stu-id="ca72a-141">String</span></span>|<span data-ttu-id="ca72a-142">スキーマ拡張機能の定義の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="ca72a-142">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="ca72a-143">値の割り当ては、以下の 2 方法のいずれかで行うことができます。</span><span class="sxs-lookup"><span data-stu-id="ca72a-143">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="ca72a-p102">確認されたドメインの内の 1 つの名前とスキーマ拡張機能の名前を連結して、\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\} という形式の一意の文字列を形成します。たとえば、`contoso_mySchema` です。 </span><span class="sxs-lookup"><span data-stu-id="ca72a-p102">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="ca72a-p103">スキーマ名を指定し、Microsoft Graph がそのスキーマ名を使用して **id** 割り当てを完了するには、次の形式を使用します。ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。たとえば、`extkvbmkofy_mySchema` です。</span><span class="sxs-lookup"><span data-stu-id="ca72a-p103">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="ca72a-148">作成後、このプロパティは変更できません。</span><span class="sxs-lookup"><span data-stu-id="ca72a-148">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="ca72a-149">owner</span><span class="sxs-lookup"><span data-stu-id="ca72a-149">owner</span></span>|<span data-ttu-id="ca72a-150">String</span><span class="sxs-lookup"><span data-stu-id="ca72a-150">String</span></span>|<span data-ttu-id="ca72a-151">スキーマ拡張機能の所有者であるアプリケーションの `appId` です。</span><span class="sxs-lookup"><span data-stu-id="ca72a-151">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="ca72a-152">このプロパティは作成時に指定して所有者を設定できます。</span><span class="sxs-lookup"><span data-stu-id="ca72a-152">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="ca72a-153">指定しない場合、呼び出し元のアプリケーションの `appId` が所有者として設定されます。</span><span class="sxs-lookup"><span data-stu-id="ca72a-153">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="ca72a-154">どちらの場合も、サインインしたユーザーがアプリケーションの所有者でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="ca72a-154">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="ca72a-155">設定すると、このプロパティは読み取り専用で、変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="ca72a-155">Once set, this property is read-only and cannot be changed.</span></span>| 
|<span data-ttu-id="ca72a-156">properties</span><span class="sxs-lookup"><span data-stu-id="ca72a-156">properties</span></span>|<span data-ttu-id="ca72a-157">[extensionSchemaProperty](extensionschemaproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ca72a-157">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="ca72a-158">スキーマ拡張機能の定義を構成するプロパティ名と種類のコレクション。</span><span class="sxs-lookup"><span data-stu-id="ca72a-158">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="ca72a-159">status</span><span class="sxs-lookup"><span data-stu-id="ca72a-159">status</span></span>|<span data-ttu-id="ca72a-160">String</span><span class="sxs-lookup"><span data-stu-id="ca72a-160">String</span></span>|<span data-ttu-id="ca72a-161">スキーマ拡張機能のライフサイクル状態。</span><span class="sxs-lookup"><span data-stu-id="ca72a-161">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="ca72a-162">考えられる状態は、**InDevelopment**、**Available**、および **Deprecated** です。</span><span class="sxs-lookup"><span data-stu-id="ca72a-162">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="ca72a-163">作成時に自動で **InDevelopment** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="ca72a-163">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="ca72a-164">考えられる状態遷移と動作の詳細については、「[スキーマ拡張機能](../../../concepts/extensibility_overview.md#schema-extensions)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="ca72a-164">[Schema extensions](../../../concepts/extensibility_overview.md#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="ca72a-165">targetTypes</span><span class="sxs-lookup"><span data-stu-id="ca72a-165">targetTypes</span></span>|<span data-ttu-id="ca72a-166">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ca72a-166">String collection</span></span>|<span data-ttu-id="ca72a-167">スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。</span><span class="sxs-lookup"><span data-stu-id="ca72a-167">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span> <span data-ttu-id="ca72a-168">**contact**、**device**、**event**、**group**、**message**、**organization**、**post**、**user** のいずれかから選択します。</span><span class="sxs-lookup"><span data-stu-id="ca72a-168">Select from **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca72a-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ca72a-169">JSON representation</span></span>

<span data-ttu-id="ca72a-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ca72a-170">Here is a JSON representation of the resource.</span></span>

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