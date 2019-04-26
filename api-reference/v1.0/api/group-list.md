---
title: グループの一覧表示
description: Office 365 グループを含み、それに限定されない組織で使用可能なすべてのグループを一覧表示します。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 8ede194abffe745bee9a23906b965d43de93cec8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561839"
---
# <a name="list-groups"></a><span data-ttu-id="6d39f-103">グループの一覧表示</span><span class="sxs-lookup"><span data-stu-id="6d39f-103">List groups</span></span>
<span data-ttu-id="6d39f-104">Office 365 グループを含み、それに限定されない組織で使用可能なすべてのグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6d39f-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="6d39f-105">この操作は既定で各グループのプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="6d39f-105">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="6d39f-106">これらの既定のプロパティは、「[プロパティ](../resources/group.md#properties)」セクションに記載されています。</span><span class="sxs-lookup"><span data-stu-id="6d39f-106">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="6d39f-107">既定で_返されない_プロパティを取得するには、グループに対して [GET](group-get.md) 操作を実行し、`$select` OData クエリ オプションでプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="6d39f-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="6d39f-108">[例](group-get.md#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d39f-108">See an [example](group-get.md#request-2).</span></span>

<span data-ttu-id="6d39f-109">例外は **hasMembersWithLicenseErrors** プロパティです。</span><span class="sxs-lookup"><span data-stu-id="6d39f-109">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="6d39f-110">このプロパティの使用方法の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d39f-110">See an [example](#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d39f-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6d39f-111">Permissions</span></span>
<span data-ttu-id="6d39f-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d39f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d39f-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d39f-114">Permission type</span></span>      | <span data-ttu-id="6d39f-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d39f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d39f-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d39f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="6d39f-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d39f-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d39f-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d39f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d39f-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d39f-119">Not supported.</span></span>    |
|<span data-ttu-id="6d39f-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d39f-120">Application</span></span> | <span data-ttu-id="6d39f-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d39f-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d39f-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d39f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d39f-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6d39f-123">Optional query parameters</span></span>
<span data-ttu-id="6d39f-124">Office 365 グループ (別名統合グループ) のみを一覧表示するには、**groupTypes** にフィルターを適用します。</span><span class="sxs-lookup"><span data-stu-id="6d39f-124">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="6d39f-125">OData クエリ オプション `$orderby` を使用して、以下の例のように、組織内のグループを **displayName** 値で並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="6d39f-125">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="6d39f-126">OData クエリ オプションの詳細については、「[OData クエリ パラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d39f-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d39f-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d39f-127">Request headers</span></span>
| <span data-ttu-id="6d39f-128">名前</span><span class="sxs-lookup"><span data-stu-id="6d39f-128">Name</span></span>       | <span data-ttu-id="6d39f-129">型</span><span class="sxs-lookup"><span data-stu-id="6d39f-129">Type</span></span> | <span data-ttu-id="6d39f-130">説明</span><span class="sxs-lookup"><span data-stu-id="6d39f-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6d39f-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d39f-131">Authorization</span></span>  | <span data-ttu-id="6d39f-132">string</span><span class="sxs-lookup"><span data-stu-id="6d39f-132">string</span></span>  | <span data-ttu-id="6d39f-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6d39f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d39f-135">要求本文</span><span class="sxs-lookup"><span data-stu-id="6d39f-135">Request body</span></span>
<span data-ttu-id="6d39f-136">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6d39f-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d39f-137">応答</span><span class="sxs-lookup"><span data-stu-id="6d39f-137">Response</span></span>
<span data-ttu-id="6d39f-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6d39f-138">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="6d39f-139">応答には、各グループの既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6d39f-139">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="6d39f-140">例</span><span class="sxs-lookup"><span data-stu-id="6d39f-140">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="6d39f-141">要求 1</span><span class="sxs-lookup"><span data-stu-id="6d39f-141">Request 1</span></span>
<span data-ttu-id="6d39f-142">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d39f-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response-1"></a><span data-ttu-id="6d39f-143">応答 1</span><span class="sxs-lookup"><span data-stu-id="6d39f-143">Response 1</span></span>
<span data-ttu-id="6d39f-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d39f-144">The following is an example of the response.</span></span>

><span data-ttu-id="6d39f-145">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6d39f-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6d39f-146">実際の呼び出しでは、各グループのすべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6d39f-146">All the default properties are returned for each group in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-12-22T02:21:05Z",
            "creationOptions": [],
            "description": "Self help community for golf",
            "displayName": "Golf Assist",
            "groupTypes": [
                "Unified"
            ],
            "mail": "golfassist@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golfassist",
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "proxyAddresses": [
                "smtp:golfassist@contoso.onmicrosoft.com",
                "SMTP:golfassist@contoso.com"
            ],
            "renewedDateTime": "2018-12-22T02:21:05Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "visibility": "Public",
            "onPremisesProvisioningErrors": []
        },
        {
            "id": "d7797254-3084-44d0-99c9-a3b5ab149538",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-11-19T20:29:40Z",
            "creationOptions": [],
            "description": "Talk about golf",
            "displayName": "Golf Discussion",
            "groupTypes": [],
            "mail": "golftalk@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golftalk",
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "proxyAddresses": [
                "smtp:golftalk@contoso.onmicrosoft.com",
                "SMTP:golftalk@contoso.com"
            ],
            "renewedDateTime": "2018-11-19T20:29:40Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "visibility": null,
            "onPremisesProvisioningErrors": []
        }
    ]
}

```
#### <a name="request-2"></a><span data-ttu-id="6d39f-147">要求 2</span><span class="sxs-lookup"><span data-stu-id="6d39f-147">Request 2</span></span>
<span data-ttu-id="6d39f-148">この例では、`$filter` クエリ オプションを使用して、グループ ベースのライセンス割り当てによるライセンス エラーが発生したメンバーが含まれているグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="6d39f-148">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="6d39f-149">また、`$select` クエリ オプションも使用して、各グループの **id** プロパティと **displayName** プロパティのみを応答で取得します (その他の既定または既定以外のプロパティは取得しません)。</span><span class="sxs-lookup"><span data-stu-id="6d39f-149">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```

#### <a name="response-2"></a><span data-ttu-id="6d39f-150">応答 2</span><span class="sxs-lookup"><span data-stu-id="6d39f-150">Response 2</span></span>
<span data-ttu-id="6d39f-151">要求したプロパティのみを含む応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d39f-151">The following is an example of the response which includes only the requested properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups_withlicenseerrors"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(id,displayName)",
    "value": [
        {
            "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
            "displayName": "Library Assist"
        },
        {
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "displayName": "Golf Assist"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
