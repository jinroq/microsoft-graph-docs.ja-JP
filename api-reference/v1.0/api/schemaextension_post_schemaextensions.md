# <a name="create-schemaextension"></a><span data-ttu-id="3e4fa-101">schemaExtension の作成</span><span class="sxs-lookup"><span data-stu-id="3e4fa-101">Create schemaExtension</span></span>

<span data-ttu-id="3e4fa-102">[サポートするリソースの種類](../../../concepts/extensibility_overview.md#supported-resources)を拡張するために、[schemaExtension](../resources/schemaextension.md) 定義を新規作成します。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-102">Create a new [schemaExtension](../resources/schemaextension.md) definition to extend a [supporting resource type](../../../concepts/extensibility_overview.md#supported-resources).</span></span>

<span data-ttu-id="3e4fa-p101">スキーマ拡張機能により、厳密に型指定されたカスタム データをリソースに追加することができます。スキーマ拡張機能を作成するアプリは、所有者アプリです。拡張機能の[状態](../../../concepts/extensibility_overview.md#schema-extensions-lifecycle)によっては、拡張機能を更新または削除できるのは、所有者アプリだけです。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-p101">Schema extensions let you add strongly-typed custom data to a resource. The app that creates a schema extension is the owner app. Depending on the [state](../../../concepts/extensibility_overview.md#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span></span> 

<span data-ttu-id="3e4fa-106">[トレーニング コースを説明するスキーマ拡張機能を定義する](../../../concepts/extensibility_schema_groups.md#2-register-a-schema-extension-definition-that-describes-a-training-course)方法、スキーマ拡張定義を使用して[トレーニング コース データで新規グループを作成する](../../../concepts/extensibility_schema_groups.md#3-create-a-new-group-with-extended-data)方法、[既存グループにトレーニング コース データを追加する](../../../concepts/extensibility_schema_groups.md#4-add-update-or-remove-custom-data-in-an-existing-group)方法については、それぞれの例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-106">See examples of how to [define a schema extension that describes a training course](../../../concepts/extensibility_schema_groups.md#2-register-a-schema-extension-definition-that-describes-a-training-course), use the schema extension definition to [create a new group with training course data](../../../concepts/extensibility_schema_groups.md#3-create-a-new-group-with-extended-data), and [add training course data to an existing group](../../../concepts/extensibility_schema_groups.md#4-add-update-or-remove-custom-data-in-an-existing-group).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e4fa-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3e4fa-107">Permissions</span></span>
<span data-ttu-id="3e4fa-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="3e4fa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3e4fa-110">Permission type</span></span>      | <span data-ttu-id="3e4fa-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3e4fa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e4fa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3e4fa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e4fa-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3e4fa-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3e4fa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3e4fa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e4fa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-115">Not supported.</span></span>    |
|<span data-ttu-id="3e4fa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3e4fa-116">Application</span></span> | <span data-ttu-id="3e4fa-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e4fa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3e4fa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a><span data-ttu-id="3e4fa-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e4fa-119">Request headers</span></span>
| <span data-ttu-id="3e4fa-120">名前</span><span class="sxs-lookup"><span data-stu-id="3e4fa-120">Name</span></span>       | <span data-ttu-id="3e4fa-121">説明</span><span class="sxs-lookup"><span data-stu-id="3e4fa-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3e4fa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e4fa-122">Authorization</span></span>  | <span data-ttu-id="3e4fa-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e4fa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e4fa-125">Content-Type</span></span>  | <span data-ttu-id="3e4fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e4fa-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e4fa-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3e4fa-127">Request body</span></span>
<span data-ttu-id="3e4fa-128">要求本文では、[schemaExtension](../resources/schemaextension.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-128">In the request body, supply a JSON representation of [schemaExtension](../resources/schemaextension.md) object.</span></span>

<span data-ttu-id="3e4fa-129">次の表に、スキーマ拡張機能の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-129">The following table shows the properties that are required when you create a schema extension.</span></span>

| <span data-ttu-id="3e4fa-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3e4fa-130">Parameter</span></span> | <span data-ttu-id="3e4fa-131">型</span><span class="sxs-lookup"><span data-stu-id="3e4fa-131">Type</span></span> | <span data-ttu-id="3e4fa-132">説明</span><span class="sxs-lookup"><span data-stu-id="3e4fa-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e4fa-133">description</span><span class="sxs-lookup"><span data-stu-id="3e4fa-133">description</span></span>|<span data-ttu-id="3e4fa-134">String</span><span class="sxs-lookup"><span data-stu-id="3e4fa-134">String</span></span>|<span data-ttu-id="3e4fa-135">スキーマ拡張機能の説明。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-135">Description for the schema extension.</span></span>|
|<span data-ttu-id="3e4fa-136">id</span><span class="sxs-lookup"><span data-stu-id="3e4fa-136">id</span></span>|<span data-ttu-id="3e4fa-137">String</span><span class="sxs-lookup"><span data-stu-id="3e4fa-137">String</span></span>|<span data-ttu-id="3e4fa-138">スキーマ拡張機能の定義の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-138">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="3e4fa-139">値の割り当ては、以下の 2 方法のいずれかで行うことができます。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-139">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="3e4fa-p104">確認されたドメインの内の 1 つの名前とスキーマ拡張機能の名前を連結して、\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\} という形式の一意の文字列を形成します。たとえば、`contoso_mySchema` です。 </span><span class="sxs-lookup"><span data-stu-id="3e4fa-p104">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="3e4fa-p105">スキーマ名を指定し、Microsoft Graph がそのスキーマ名を使用して **id** 割り当てを完了するには、次の形式を使用します。ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。たとえば、`extkvbmkofy_mySchema` です。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="3e4fa-144">作成後、このプロパティは変更できません。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-144">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="3e4fa-145">properties</span><span class="sxs-lookup"><span data-stu-id="3e4fa-145">properties</span></span>|<span data-ttu-id="3e4fa-146">[extensionSchemaProperty](../resources/extensionschemaproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3e4fa-146">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="3e4fa-147">スキーマ拡張機能の定義を構成するプロパティの名前と種類のコレクション。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-147">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="3e4fa-148">targetTypes</span><span class="sxs-lookup"><span data-stu-id="3e4fa-148">targetTypes</span></span>|<span data-ttu-id="3e4fa-149">String collection</span><span class="sxs-lookup"><span data-stu-id="3e4fa-149">String collection</span></span>|<span data-ttu-id="3e4fa-150">このスキーマ拡張機能の定義を適用できる、(スキーマ拡張機能をサポートしている) 一連の Microsoft Graph のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-150">Set of Microsoft Graph resource types (that support schema extensions) that this schema extension definition can be applied to.</span></span>|

## <a name="response"></a><span data-ttu-id="3e4fa-151">応答</span><span class="sxs-lookup"><span data-stu-id="3e4fa-151">Response</span></span>

<span data-ttu-id="3e4fa-152">成功した場合、このメソッドは応答本文で `201, Created` 応答コードと、[schemaExtension](../resources/schemaextension.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-152">If successful, this method returns `201, Created` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e4fa-153">例</span><span class="sxs-lookup"><span data-stu-id="3e4fa-153">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="3e4fa-154">要求 1</span><span class="sxs-lookup"><span data-stu-id="3e4fa-154">Request 1</span></span>

<span data-ttu-id="3e4fa-p106">最初の例では、確認済みのドメイン名 `graphlearn` とスキーマ名 `courses` を使用して、スキーマ拡張機能の定義の **id** プロパティの一意の文字列を形成します。一意の文字列は次の形式に基づきます。\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-p106">The first example shows using a verified domain name, `graphlearn`, and a schema name, `courses`, to form a unique string for the **id** property of the schema extension definition. The unique string is based on this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span>

<span data-ttu-id="3e4fa-157">要求本文では、[schemaExtension](../resources/schemaextension.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-157">In the request body, supply a JSON representation of the [schemaExtension](../resources/schemaextension.md) object.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
Content-type: application/json

{
    "id":"graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="response-1"></a><span data-ttu-id="3e4fa-158">応答 1</span><span class="sxs-lookup"><span data-stu-id="3e4fa-158">Response 1</span></span>

<span data-ttu-id="3e4fa-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="3e4fa-162">要求 2</span><span class="sxs-lookup"><span data-stu-id="3e4fa-162">Request 2</span></span>

<span data-ttu-id="3e4fa-p108">2 番目の例では、要求の **id** プロパティ内のスキーマ名 `courses` だけを指定し、[schemaExtension](../resources/schemaextension.md) オブジェクト内の残りのプロパティを JSON 表記で指定しています。Microsoft Graph は一意の文字列値を割り当て、それを応答内で返します。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-p108">The second example shows specifying just a schema name, `courses`, in the **id** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object. Microsoft Graph will assign and return a unique string value in the response.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
Content-type: application/json

{
    "id":"courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="3e4fa-165">応答 2</span><span class="sxs-lookup"><span data-stu-id="3e4fa-165">Response 2</span></span>

<span data-ttu-id="3e4fa-p109">応答には、要求の中で提供されているスキーマ名に基づいた一意の文字列がその **id** プロパティ内に含まれ、新規作成したスキーマ定義の残りの部分も応答に含まれています。応答の中の **id** の値は、次の形式に基づきます。ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3e4fa-p109">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition. The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "extk9eruy7c_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```


## <a name="see-also"></a><span data-ttu-id="3e4fa-170">関連項目</span><span class="sxs-lookup"><span data-stu-id="3e4fa-170">See also</span></span>

- [<span data-ttu-id="3e4fa-171">拡張機能を使用したリソースへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="3e4fa-171">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="3e4fa-172">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="3e4fa-172">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->