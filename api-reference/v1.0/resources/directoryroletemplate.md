---
title: directoryRoleTemplate リソース型
description: ディレクトリ ロール テンプレートを表します。 ディレクトリ ロール テンプレートでは、ディレクトリ ロール (directoryRole) のプロパティ値を指定します。 テナントでアクティブにすることがあるディレクトリの役割ごとに、関連付けられているディレクトリ ロール テンプレート オブジェクトがあります。 ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。 既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。 他の使用可能なディレクトリロールをアクティブ化するには`/directoryRoles` 、要求の**roleTemplateId**パラメーターでディレクトリロールが指定されているディレクトリロールテンプレートの ID を使用して、POST 要求をエンドポイントに送信します。 この ID は、要求の roleTemplateId パラメーターで指定したディレクトリ ロールに基づきます。 この要求が正常に完了すると、ディレクトリ ロールの読み取りや、ディレクトリ ロールへのメンバーの追加ができるようになります。**注**:ディレクトリ ロール テンプレートは、ユーザー (Users) ディレクトリ ロールに公開されます。 ユーザー ディレクトリ ロールは、暗黙的であり、ディレクトリ クライアントには表示されません。 テナント内のすべてのユーザーは、インフラストラクチャによって、このロールに割り当てられます。 このロールは、あらかじめアクティブ化されています。 このテンプレートは、使用しないでください。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5480e32498b4503cf4119b56c1025979c383a21c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029450"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="6335c-114">directoryRoleTemplate リソース型</span><span class="sxs-lookup"><span data-stu-id="6335c-114">directoryRoleTemplate resource type</span></span>

<span data-ttu-id="6335c-p102">ディレクトリ ロール テンプレートを表します。ディレクトリ ロール テンプレートでは、ディレクトリ ロール ([directoryRole](directoryrole.md)) のプロパティ値を指定します。テナントでアクティブにすることがあるディレクトリの役割ごとに、関連付けられているディレクトリ ロール テンプレート オブジェクトがあります。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。その他の使用可能なディレクトリ ロールをアクティブ化するには、ディレクトリ ロール テンプレートの ID を使用して `/directoryRoles` エンドポイントに POST 要求を送信します。この ID は、要求の **roleTemplateId** パラメーターで指定したディレクトリ ロールに基づきます。この要求が正常に完了すると、ディレクトリ ロールの読み取りや、ディレクトリ ロールへのメンバーの追加ができるようになります。**注**:ディレクトリ ロール テンプレートは、ユーザー (Users) ディレクトリ ロールに公開されます。ユーザー ディレクトリ ロールは、暗黙的であり、ディレクトリ クライアントには表示されません。テナント内のすべてのユーザーは、インフラストラクチャによって、このロールに割り当てられます。このロールは、あらかじめアクティブ化されています。このテンプレートは、使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="6335c-p102">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="6335c-127">メソッド</span><span class="sxs-lookup"><span data-stu-id="6335c-127">Methods</span></span>

| <span data-ttu-id="6335c-128">メソッド</span><span class="sxs-lookup"><span data-stu-id="6335c-128">Method</span></span>       | <span data-ttu-id="6335c-129">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6335c-129">Return Type</span></span>  |<span data-ttu-id="6335c-130">説明</span><span class="sxs-lookup"><span data-stu-id="6335c-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6335c-131">Get directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="6335c-131">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="6335c-132">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="6335c-132">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="6335c-133">directoryRoleTemplate オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6335c-133">Read properties and relationships of directoryRoleTemplate object.</span></span>|
|[<span data-ttu-id="6335c-134">List directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="6335c-134">List directoryRoleTemplate</span></span>](../api/directoryroletemplate-list.md) | <span data-ttu-id="6335c-135">[directoryRoleTemplate](directoryroletemplate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6335c-135">[directoryRoleTemplate](directoryroletemplate.md) collection</span></span> |<span data-ttu-id="6335c-136">directoryRoleTemplate オブジェクトのリストを取得します</span><span class="sxs-lookup"><span data-stu-id="6335c-136">Retrieve a list of directoryRoleTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="6335c-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6335c-137">Properties</span></span>
| <span data-ttu-id="6335c-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6335c-138">Property</span></span>     | <span data-ttu-id="6335c-139">型</span><span class="sxs-lookup"><span data-stu-id="6335c-139">Type</span></span>   |<span data-ttu-id="6335c-140">説明</span><span class="sxs-lookup"><span data-stu-id="6335c-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6335c-141">description</span><span class="sxs-lookup"><span data-stu-id="6335c-141">description</span></span>|<span data-ttu-id="6335c-142">String</span><span class="sxs-lookup"><span data-stu-id="6335c-142">String</span></span>|<span data-ttu-id="6335c-p103">ディレクトリ ロールに設定する説明。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6335c-p103">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="6335c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6335c-145">displayName</span></span>|<span data-ttu-id="6335c-146">String</span><span class="sxs-lookup"><span data-stu-id="6335c-146">String</span></span>|<span data-ttu-id="6335c-p104">ディレクトリ ロールに設定する表示名。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6335c-p104">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="6335c-149">id</span><span class="sxs-lookup"><span data-stu-id="6335c-149">id</span></span>|<span data-ttu-id="6335c-150">文字列</span><span class="sxs-lookup"><span data-stu-id="6335c-150">String</span></span>|<span data-ttu-id="6335c-p105">テンプレートの一意識別子。[directoryObject](directoryobject.md) から継承されます。POST 要求の **roleTemplateId** プロパティにディレクトリ ロール テンプレートの **id** を指定して、テナントの [directoryRole](directoryrole.md) をアクティブ化します。キーであり、Null は許容されません。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6335c-p105">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6335c-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6335c-156">Relationships</span></span>
<span data-ttu-id="6335c-157">なし</span><span class="sxs-lookup"><span data-stu-id="6335c-157">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="6335c-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6335c-158">JSON representation</span></span>

<span data-ttu-id="6335c-159">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6335c-159">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
