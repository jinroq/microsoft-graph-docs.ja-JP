---
title: directoryRoleTemplate リソース型
description: ディレクトリ ロール テンプレートを表します。ディレクトリ ロール テンプレートでは、ディレクトリ ロール (directoryRole) のプロパティ値を指定します。テナントでアクティブにすることがあるディレクトリの役割ごとに、関連付けられているディレクトリ ロール テンプレート オブジェクトがあります。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。その他の使用可能なディレクトリ ロールをアクティブ化するには、ディレクトリ ロール テンプレートの ID を使用して  エンドポイントに POST 要求を送信します。この ID は、要求の roleTemplateId パラメーターで指定したディレクトリ ロールに基づきます。この要求が正常に完了すると、ディレクトリ ロールの読み取りや、ディレクトリ ロールへのメンバーの追加ができるようになります。注:ディレクトリ ロール テンプレートは、ユーザー (Users) ディレクトリ ロールに公開されます。ユーザー ディレクトリ ロールは、暗黙的であり、ディレクトリ クライアントには表示されません。テナント内のすべてのユーザーは、インフラストラクチャによって、このロールに割り当てられます。このロールは、あらかじめアクティブ化されています。このテンプレートは、使用しないでください。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd813c9f7676e7190e5aedbb6d9b950e9ffc6aac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526159"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="f46a4-114">directoryRoleTemplate リソース型</span><span class="sxs-lookup"><span data-stu-id="f46a4-114">directoryRoleTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f46a4-p102">ディレクトリ ロール テンプレートを表します。ディレクトリ ロール テンプレートでは、ディレクトリ ロール ([directoryRole](directoryrole.md)) のプロパティ値を指定します。テナントでアクティブにすることがあるディレクトリの役割ごとに、関連付けられているディレクトリ ロール テンプレート オブジェクトがあります。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。その他の使用可能なディレクトリ ロールをアクティブ化するには、ディレクトリ ロール テンプレートの ID を使用して `/directoryRoles` エンドポイントに POST 要求を送信します。この ID は、要求の **roleTemplateId** パラメーターで指定したディレクトリ ロールに基づきます。この要求が正常に完了すると、ディレクトリ ロールの読み取りや、ディレクトリ ロールへのメンバーの追加ができるようになります。**注**:ディレクトリ ロール テンプレートは、ユーザー (Users) ディレクトリ ロールに公開されます。ユーザー ディレクトリ ロールは、暗黙的であり、ディレクトリ クライアントには表示されません。テナント内のすべてのユーザーは、インフラストラクチャによって、このロールに割り当てられます。このロールは、あらかじめアクティブ化されています。このテンプレートは、使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="f46a4-p102">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="f46a4-127">メソッド</span><span class="sxs-lookup"><span data-stu-id="f46a4-127">Methods</span></span>

| <span data-ttu-id="f46a4-128">メソッド</span><span class="sxs-lookup"><span data-stu-id="f46a4-128">Method</span></span>       | <span data-ttu-id="f46a4-129">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f46a4-129">Return Type</span></span>  |<span data-ttu-id="f46a4-130">説明</span><span class="sxs-lookup"><span data-stu-id="f46a4-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f46a4-131">Get directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="f46a4-131">[Get directoryRoleTemplate](../api/directoryroletemplate-get.md)</span></span> | [<span data-ttu-id="f46a4-132">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="f46a4-132">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="f46a4-133">directoryRoleTemplate オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f46a4-133">Read properties and relationships of directoryRoleTemplate object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f46a4-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f46a4-134">Properties</span></span>
| <span data-ttu-id="f46a4-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f46a4-135">Property</span></span>     | <span data-ttu-id="f46a4-136">型</span><span class="sxs-lookup"><span data-stu-id="f46a4-136">Type</span></span>   |<span data-ttu-id="f46a4-137">説明</span><span class="sxs-lookup"><span data-stu-id="f46a4-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f46a4-138">説明</span><span class="sxs-lookup"><span data-stu-id="f46a4-138">description</span></span>|<span data-ttu-id="f46a4-139">String</span><span class="sxs-lookup"><span data-stu-id="f46a4-139">String</span></span>|<span data-ttu-id="f46a4-p103">ディレクトリ ロールに設定する説明。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f46a4-p103">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="f46a4-142">displayName</span><span class="sxs-lookup"><span data-stu-id="f46a4-142">displayName</span></span>|<span data-ttu-id="f46a4-143">String</span><span class="sxs-lookup"><span data-stu-id="f46a4-143">String</span></span>|<span data-ttu-id="f46a4-p104">ディレクトリ ロールに設定する表示名。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f46a4-p104">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="f46a4-146">id</span><span class="sxs-lookup"><span data-stu-id="f46a4-146">id</span></span>|<span data-ttu-id="f46a4-147">文字列</span><span class="sxs-lookup"><span data-stu-id="f46a4-147">String</span></span>|<span data-ttu-id="f46a4-p105">テンプレートの一意識別子。[directoryObject](directoryobject.md) から継承されます。POST 要求の **roleTemplateId** プロパティにディレクトリ ロール テンプレートの **id** を指定して、テナントの [directoryRole](directoryrole.md) をアクティブ化します。キーであり、Null は許容されません。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f46a4-p105">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f46a4-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f46a4-153">Relationships</span></span>
<span data-ttu-id="f46a4-154">なし</span><span class="sxs-lookup"><span data-stu-id="f46a4-154">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="f46a4-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f46a4-155">JSON representation</span></span>

<span data-ttu-id="f46a4-156">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f46a4-156">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryroletemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
