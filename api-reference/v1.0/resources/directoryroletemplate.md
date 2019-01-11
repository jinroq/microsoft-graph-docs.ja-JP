---
title: directoryRoleTemplate リソース型
description: 'ディレクトリの役割のテンプレートを表します。 ロール テンプレート ディレクトリは、ディレクトリの役割 (directoryRole) のプロパティ値を指定します。 テナントでアクティブにすることがあるディレクトリの役割ごとに、関連付けられているディレクトリ ロール テンプレート オブジェクトがあります。 ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。 会社の管理者のディレクトリの役割のみが既定でアクティブにします。 POST 要求を送信するその他の利用可能なディレクトリの役割を有効にするのには、`/directoryRoles`の要求の**roleTemplateId**パラメーターで指定されたディレクトリの役割の基になるディレクトリ ロール テンプレートの ID を持つエンドポイントです。 この要求の完了時に読み取りとディレクトリのロールにメンバーを割り当てるし、開始できます。 **注**: このロールに、ユーザー ディレクトリのディレクトリの役割のテンプレートが公開されています。 ユーザー ディレクトリの役割は、暗黙の型がクライアントのディレクトリに表示されていません。 テナントのすべてのユーザーは、インフラストラクチャによって、このロールに割り当てられます。 ロールが既にアクティブになっています。 このテンプレートを使用しません。'
localization_priority: Normal
ms.openlocfilehash: 0603ee4424cf651c37bc1790b378c1472ba99216
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811460"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="24194-114">directoryRoleTemplate リソース型</span><span class="sxs-lookup"><span data-stu-id="24194-114">directoryRoleTemplate resource type</span></span>

<span data-ttu-id="24194-p102">ディレクトリ ロール テンプレートを表します。ディレクトリ ロール テンプレートでは、ディレクトリ ロール ([directoryRole](directoryrole.md)) のプロパティ値を指定します。テナントでアクティブにすることがあるディレクトリの役割ごとに、関連付けられているディレクトリ ロール テンプレート オブジェクトがあります。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。その他の使用可能なディレクトリ ロールをアクティブ化するには、ディレクトリ ロール テンプレートの ID を使用して `/directoryRoles` エンドポイントに POST 要求を送信します。この ID は、要求の **roleTemplateId** パラメーターで指定したディレクトリ ロールに基づきます。この要求が正常に完了すると、ディレクトリ ロールの読み取りや、ディレクトリ ロールへのメンバーの追加ができるようになります。**注**:ディレクトリ ロール テンプレートは、ユーザー (Users) ディレクトリ ロールに公開されます。ユーザー ディレクトリ ロールは、暗黙的であり、ディレクトリ クライアントには表示されません。テナント内のすべてのユーザーは、インフラストラクチャによって、このロールに割り当てられます。このロールは、あらかじめアクティブ化されています。このテンプレートは、使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="24194-p102">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="24194-127">メソッド</span><span class="sxs-lookup"><span data-stu-id="24194-127">Methods</span></span>

| <span data-ttu-id="24194-128">メソッド</span><span class="sxs-lookup"><span data-stu-id="24194-128">Method</span></span>       | <span data-ttu-id="24194-129">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="24194-129">Return Type</span></span>  |<span data-ttu-id="24194-130">説明</span><span class="sxs-lookup"><span data-stu-id="24194-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="24194-131">Get directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="24194-131">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="24194-132">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="24194-132">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="24194-133">directoryRoleTemplate オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="24194-133">Read properties and relationships of directoryRoleTemplate object.</span></span>|
|[<span data-ttu-id="24194-134">directoryRoleTemplate を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="24194-134">List directoryRoleTemplate</span></span>](../api/directoryroletemplate-list.md) | <span data-ttu-id="24194-135">[directoryRoleTemplate](directoryroletemplate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="24194-135">[directoryRoleTemplate](directoryroletemplate.md) collection</span></span> |<span data-ttu-id="24194-136">directoryRoleTemplate オブジェクトのリストを取得します</span><span class="sxs-lookup"><span data-stu-id="24194-136">Retrieve a list of directoryRoleTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="24194-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24194-137">Properties</span></span>
| <span data-ttu-id="24194-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24194-138">Property</span></span>     | <span data-ttu-id="24194-139">種類</span><span class="sxs-lookup"><span data-stu-id="24194-139">Type</span></span>   |<span data-ttu-id="24194-140">説明</span><span class="sxs-lookup"><span data-stu-id="24194-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24194-141">説明</span><span class="sxs-lookup"><span data-stu-id="24194-141">description</span></span>|<span data-ttu-id="24194-142">String</span><span class="sxs-lookup"><span data-stu-id="24194-142">String</span></span>|<span data-ttu-id="24194-p103">ディレクトリ ロールに設定する説明。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="24194-p103">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="24194-145">displayName</span><span class="sxs-lookup"><span data-stu-id="24194-145">displayName</span></span>|<span data-ttu-id="24194-146">String</span><span class="sxs-lookup"><span data-stu-id="24194-146">String</span></span>|<span data-ttu-id="24194-p104">ディレクトリ ロールに設定する表示名。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="24194-p104">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="24194-149">id</span><span class="sxs-lookup"><span data-stu-id="24194-149">id</span></span>|<span data-ttu-id="24194-150">String</span><span class="sxs-lookup"><span data-stu-id="24194-150">String</span></span>|<span data-ttu-id="24194-p105">テンプレートの一意識別子。[directoryObject](directoryobject.md) から継承されます。POST 要求の **roleTemplateId** プロパティにディレクトリ ロール テンプレートの **id** を指定して、テナントの [directoryRole](directoryrole.md) をアクティブ化します。キーであり、Null は許容されません。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="24194-p105">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24194-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="24194-156">Relationships</span></span>
<span data-ttu-id="24194-157">なし</span><span class="sxs-lookup"><span data-stu-id="24194-157">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="24194-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24194-158">JSON representation</span></span>

<span data-ttu-id="24194-159">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="24194-159">Here is a JSON representation of the resource</span></span>

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
