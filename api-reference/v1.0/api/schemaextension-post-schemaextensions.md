---
title: schemaExtension の作成
description: サポートするリソースの種類を拡張するために、schemaExtension 定義を新規作成します。
ms.openlocfilehash: b66cdc9d589520bbdf3557c4d1ea791f75def984
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021629"
---
# <a name="create-schemaextension"></a><span data-ttu-id="a07f4-103">schemaExtension の作成</span><span class="sxs-lookup"><span data-stu-id="a07f4-103">Create schemaExtension</span></span>

<span data-ttu-id="a07f4-104">[サポートするリソースの種類](/graph/extensibility-overview#supported-resources)を拡張するために、[schemaExtension](../resources/schemaextension.md) 定義を新規作成します。</span><span class="sxs-lookup"><span data-stu-id="a07f4-104">Create a new [schemaExtension](../resources/schemaextension.md) definition to extend a [supporting resource type](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="a07f4-p101">スキーマ拡張機能により、厳密に型指定されたカスタム データをリソースに追加することができます。スキーマ拡張機能を作成するアプリは、所有者アプリです。拡張機能の[状態](/graph/extensibility-overview#schema-extensions-lifecycle)によっては、拡張機能を更新または削除できるのは、所有者アプリだけです。</span><span class="sxs-lookup"><span data-stu-id="a07f4-p101">Schema extensions let you add strongly-typed custom data to a resource. The app that creates a schema extension is the owner app. Depending on the [state](/graph/extensibility-overview#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span></span> 

<span data-ttu-id="a07f4-108">[トレーニング コースを説明するスキーマ拡張機能を定義する](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course)方法、スキーマ拡張定義を使用して[トレーニング コース データで新規グループを作成する](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data)方法、[既存グループにトレーニング コース データを追加する](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group)方法については、それぞれの例を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a07f4-108">See examples of how to [define a schema extension that describes a training course](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), use the schema extension definition to [create a new group with training course data](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data), and [add training course data to an existing group](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span></span>

## <a name="permissions"></a><span data-ttu-id="a07f4-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a07f4-109">Permissions</span></span>
<span data-ttu-id="a07f4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a07f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a07f4-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a07f4-112">Permission type</span></span>      | <span data-ttu-id="a07f4-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a07f4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a07f4-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a07f4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a07f4-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a07f4-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a07f4-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a07f4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a07f4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a07f4-117">Not supported.</span></span>    |
|<span data-ttu-id="a07f4-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a07f4-118">Application</span></span> | <span data-ttu-id="a07f4-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a07f4-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a07f4-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a07f4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a><span data-ttu-id="a07f4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a07f4-121">Request headers</span></span>
| <span data-ttu-id="a07f4-122">名前</span><span class="sxs-lookup"><span data-stu-id="a07f4-122">Name</span></span>       | <span data-ttu-id="a07f4-123">説明</span><span class="sxs-lookup"><span data-stu-id="a07f4-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a07f4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a07f4-124">Authorization</span></span>  | <span data-ttu-id="a07f4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a07f4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a07f4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a07f4-127">Content-Type</span></span>  | <span data-ttu-id="a07f4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a07f4-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a07f4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="a07f4-129">Request body</span></span>
<span data-ttu-id="a07f4-130">要求本文では、[schemaExtension](../resources/schemaextension.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a07f4-130">In the request body, supply a JSON representation of [schemaExtension](../resources/schemaextension.md) object.</span></span>

<span data-ttu-id="a07f4-131">次の表に、スキーマ拡張機能の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a07f4-131">The following table shows the properties that are required when you create a schema extension.</span></span>

| <span data-ttu-id="a07f4-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="a07f4-132">Parameter</span></span> | <span data-ttu-id="a07f4-133">型</span><span class="sxs-lookup"><span data-stu-id="a07f4-133">Type</span></span> | <span data-ttu-id="a07f4-134">説明</span><span class="sxs-lookup"><span data-stu-id="a07f4-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a07f4-135">説明</span><span class="sxs-lookup"><span data-stu-id="a07f4-135">description</span></span>|<span data-ttu-id="a07f4-136">String</span><span class="sxs-lookup"><span data-stu-id="a07f4-136">String</span></span>|<span data-ttu-id="a07f4-137">スキーマ拡張機能の説明。</span><span class="sxs-lookup"><span data-stu-id="a07f4-137">Description for the schema extension.</span></span>|
|<span data-ttu-id="a07f4-138">id</span><span class="sxs-lookup"><span data-stu-id="a07f4-138">id</span></span>|<span data-ttu-id="a07f4-139">String</span><span class="sxs-lookup"><span data-stu-id="a07f4-139">String</span></span>|<span data-ttu-id="a07f4-140">スキーマ拡張機能の定義の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a07f4-140">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="a07f4-141">値の割り当ては、以下の 2 方法のいずれかで行うことができます。</span><span class="sxs-lookup"><span data-stu-id="a07f4-141">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="a07f4-142">確認されたドメインの内の 1 つの名前とスキーマ拡張機能の名前を連結して、\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\} という形式の一意の文字列を形成します。</span><span class="sxs-lookup"><span data-stu-id="a07f4-142">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span> <span data-ttu-id="a07f4-143">次に例 `contoso_mySchema` を示します。</span><span class="sxs-lookup"><span data-stu-id="a07f4-143">As an example, `contoso_mySchema`.</span></span> <span data-ttu-id="a07f4-144">注: 上位ドメイン `.com`、`.net`、`.gov`、`.edu`、`.org` の下では、検証済みのドメインのみがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="a07f4-144">NOTE: Only verified domains under the following top-level domains are supported: `.com`,`.net`, `.gov`, `.edu` or `.org`.</span></span> </li><li><span data-ttu-id="a07f4-p105">スキーマ名を指定し、Microsoft Graph がそのスキーマ名を使用して **id** 割り当てを完了するには、次の形式を使用します。ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。たとえば、`extkvbmkofy_mySchema` です。</span><span class="sxs-lookup"><span data-stu-id="a07f4-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="a07f4-147">作成後、このプロパティは変更できません。</span><span class="sxs-lookup"><span data-stu-id="a07f4-147">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="a07f4-148">owner</span><span class="sxs-lookup"><span data-stu-id="a07f4-148">owner</span></span>|<span data-ttu-id="a07f4-149">String</span><span class="sxs-lookup"><span data-stu-id="a07f4-149">String</span></span>|<span data-ttu-id="a07f4-150">(省略可能) スキーマ拡張機能の所有者であるアプリケーションの `appId` です。</span><span class="sxs-lookup"><span data-stu-id="a07f4-150">(Optional) The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="a07f4-151">このプロパティは作成時に指定して所有者を設定できます。</span><span class="sxs-lookup"><span data-stu-id="a07f4-151">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="a07f4-152">指定しない場合、呼び出し元のアプリケーションの `appId` が所有者として設定されます。</span><span class="sxs-lookup"><span data-stu-id="a07f4-152">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="a07f4-153">たとえば、Graph エクスプローラーを使用して新しいスキーマ拡張機能の定義を作成する場合は、所有者プロパティを指定する**必要があります**。</span><span class="sxs-lookup"><span data-stu-id="a07f4-153">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property.</span></span> <span data-ttu-id="a07f4-154">設定すると、このプロパティは読み取り専用で、変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="a07f4-154">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="a07f4-155">properties</span><span class="sxs-lookup"><span data-stu-id="a07f4-155">properties</span></span>|<span data-ttu-id="a07f4-156">[extensionSchemaProperty](../resources/extensionschemaproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a07f4-156">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="a07f4-157">スキーマ拡張機能の定義を構成するプロパティの名前と種類のコレクション。</span><span class="sxs-lookup"><span data-stu-id="a07f4-157">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="a07f4-158">targetTypes</span><span class="sxs-lookup"><span data-stu-id="a07f4-158">targetTypes</span></span>|<span data-ttu-id="a07f4-159">String collection</span><span class="sxs-lookup"><span data-stu-id="a07f4-159">String collection</span></span>|<span data-ttu-id="a07f4-160">このスキーマ拡張機能の定義を適用できる、(スキーマ拡張機能をサポートしている) 一連の Microsoft Graph のリソースの種類。</span><span class="sxs-lookup"><span data-stu-id="a07f4-160">Set of Microsoft Graph resource types (that support schema extensions) that this schema extension definition can be applied to.</span></span>|

## <a name="response"></a><span data-ttu-id="a07f4-161">応答</span><span class="sxs-lookup"><span data-stu-id="a07f4-161">Response</span></span>

<span data-ttu-id="a07f4-162">成功した場合、このメソッドは応答本文で `201 Created` 応答コードと、[schemaExtension](../resources/schemaextension.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a07f4-162">If successful, this method returns `201 Created` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a07f4-163">例</span><span class="sxs-lookup"><span data-stu-id="a07f4-163">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="a07f4-164">要求 1</span><span class="sxs-lookup"><span data-stu-id="a07f4-164">Request 1</span></span>

<span data-ttu-id="a07f4-p107">最初の例では、確認済みのドメイン名 `graphlearn` とスキーマ名 `courses` を使用して、スキーマ拡張機能の定義の **id** プロパティの一意の文字列を形成します。一意の文字列は次の形式に基づきます。\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。</span><span class="sxs-lookup"><span data-stu-id="a07f4-p107">The first example shows using a verified domain name, `graphlearn`, and a schema name, `courses`, to form a unique string for the **id** property of the schema extension definition. The unique string is based on this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span>

<span data-ttu-id="a07f4-167">要求本文では、[schemaExtension](../resources/schemaextension.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a07f4-167">In the request body, supply a JSON representation of the [schemaExtension](../resources/schemaextension.md) object.</span></span>
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

##### <a name="response-1"></a><span data-ttu-id="a07f4-168">応答 1</span><span class="sxs-lookup"><span data-stu-id="a07f4-168">Response 1</span></span>

<span data-ttu-id="a07f4-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a07f4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="a07f4-172">要求 2</span><span class="sxs-lookup"><span data-stu-id="a07f4-172">Request 2</span></span>

<span data-ttu-id="a07f4-p109">2 番目の例では、要求の **id** プロパティ内のスキーマ名 `courses` だけを指定し、[schemaExtension](../resources/schemaextension.md) オブジェクト内の残りのプロパティを JSON 表記で指定しています。Microsoft Graph は一意の文字列値を割り当て、それを応答内で返します。</span><span class="sxs-lookup"><span data-stu-id="a07f4-p109">The second example shows specifying just a schema name, `courses`, in the **id** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object. Microsoft Graph will assign and return a unique string value in the response.</span></span>

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

##### <a name="response-2"></a><span data-ttu-id="a07f4-175">応答 2</span><span class="sxs-lookup"><span data-stu-id="a07f4-175">Response 2</span></span>

<span data-ttu-id="a07f4-p110">応答には、要求の中で提供されているスキーマ名に基づいた一意の文字列がその **id** プロパティ内に含まれ、新規作成したスキーマ定義の残りの部分も応答に含まれています。応答の中の **id** の値は、次の形式に基づきます。ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a07f4-p110">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition. The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="a07f4-180">関連項目</span><span class="sxs-lookup"><span data-stu-id="a07f4-180">See also</span></span>

- [<span data-ttu-id="a07f4-181">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="a07f4-181">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a07f4-182">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="a07f4-182">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->