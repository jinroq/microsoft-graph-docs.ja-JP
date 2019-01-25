---
title: グループの一覧表示
description: Office 365 グループを含み、それに限定されない組織で使用可能なすべてのグループを一覧表示します。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5081c5013c1bf7c1a1bfbcff58afe5a83aa67bc9
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726576"
---
# <a name="list-groups"></a><span data-ttu-id="e3aa8-103">グループの一覧表示</span><span class="sxs-lookup"><span data-stu-id="e3aa8-103">List groups</span></span>
<span data-ttu-id="e3aa8-104">Office 365 グループを含み、それに限定されない組織で使用可能なすべてのグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="e3aa8-105">この操作は既定で各グループのプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-105">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="e3aa8-106">これらの既定のプロパティは、「[プロパティ](../resources/group.md#properties)」セクションに記載されています。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-106">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="e3aa8-107">既定で_返されない_プロパティを取得するには、グループに対して [GET](group-get.md) 操作を実行し、`$select` OData クエリ オプションでプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="e3aa8-108">[例](group-get.md#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-108">See an [example](group-get.md#request-2).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3aa8-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3aa8-109">Permissions</span></span>
<span data-ttu-id="e3aa8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3aa8-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3aa8-112">Permission type</span></span>      | <span data-ttu-id="e3aa8-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3aa8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3aa8-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3aa8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e3aa8-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3aa8-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3aa8-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3aa8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3aa8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-117">Not supported.</span></span>    |
|<span data-ttu-id="e3aa8-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3aa8-118">Application</span></span> | <span data-ttu-id="e3aa8-119">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3aa8-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3aa8-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3aa8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3aa8-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e3aa8-121">Optional query parameters</span></span>
<span data-ttu-id="e3aa8-122">Office 365 グループ (別名統合グループ) のみを一覧表示するには、**groupTypes** にフィルターを適用します。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="e3aa8-122">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="e3aa8-123">次の例のように、OData クエリ オプション `$orderby` を使用して、組織内のグループを **displayName** 値で並べ替えることができます。<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="e3aa8-123">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="e3aa8-124">OData クエリ オプションの詳細については、「[OData クエリ パラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3aa8-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3aa8-125">Request headers</span></span>
| <span data-ttu-id="e3aa8-126">名前</span><span class="sxs-lookup"><span data-stu-id="e3aa8-126">Name</span></span>       | <span data-ttu-id="e3aa8-127">型</span><span class="sxs-lookup"><span data-stu-id="e3aa8-127">Type</span></span> | <span data-ttu-id="e3aa8-128">説明</span><span class="sxs-lookup"><span data-stu-id="e3aa8-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e3aa8-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3aa8-129">Authorization</span></span>  | <span data-ttu-id="e3aa8-130">string</span><span class="sxs-lookup"><span data-stu-id="e3aa8-130">string</span></span>  | <span data-ttu-id="e3aa8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3aa8-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3aa8-133">Request body</span></span>
<span data-ttu-id="e3aa8-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3aa8-135">応答</span><span class="sxs-lookup"><span data-stu-id="e3aa8-135">Response</span></span>
<span data-ttu-id="e3aa8-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="e3aa8-137">応答には、各グループの既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-137">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="e3aa8-138">例</span><span class="sxs-lookup"><span data-stu-id="e3aa8-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e3aa8-139">要求</span><span class="sxs-lookup"><span data-stu-id="e3aa8-139">Request</span></span>
<span data-ttu-id="e3aa8-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="e3aa8-141">応答</span><span class="sxs-lookup"><span data-stu-id="e3aa8-141">Response</span></span>
<span data-ttu-id="e3aa8-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-142">The following is an example of the response.</span></span>

><span data-ttu-id="e3aa8-143">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e3aa8-144">実際の呼び出しでは、各グループのすべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e3aa8-144">All the default properties are returned for each group in an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
