---
title: GovernanceRoleAssignmentRequests のエクスポート
description: ブラウザーで .csv ファイルとして解析`application/octet-stream`できる形式で governanceRoleAssignmentRequests のコレクションを取得します。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 227968ab265c117e5fa297d8fd8d8a988ddd0028
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954285"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="79fad-103">GovernanceRoleAssignmentRequests のエクスポート</span><span class="sxs-lookup"><span data-stu-id="79fad-103">Export governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79fad-104">ブラウザーで .csv ファイル[](../resources/governanceroleassignmentrequest.md)として解析`application/octet-stream`できる形式で governanceRoleAssignmentRequests のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="79fad-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="79fad-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79fad-105">Permissions</span></span>
<span data-ttu-id="79fad-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79fad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79fad-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79fad-108">Permission type</span></span>      | <span data-ttu-id="79fad-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79fad-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79fad-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79fad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="79fad-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="79fad-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="79fad-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79fad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79fad-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79fad-113">Not supported.</span></span>    |
|<span data-ttu-id="79fad-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79fad-114">Application</span></span> | <span data-ttu-id="79fad-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79fad-115">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="79fad-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79fad-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="79fad-117">[GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションをリソースにエクスポートする</span><span class="sxs-lookup"><span data-stu-id="79fad-117">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="79fad-118">**注:** この要求では、アクセス許可スコープの他に、リソースに対して少なくとも1つの役割の割り当てが必要になります。</span><span class="sxs-lookup"><span data-stu-id="79fad-118">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="79fad-119">[GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションをエクスポートする</span><span class="sxs-lookup"><span data-stu-id="79fad-119">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="79fad-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="79fad-120">Optional query parameters</span></span>
<span data-ttu-id="79fad-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="79fad-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79fad-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79fad-122">Request headers</span></span>
| <span data-ttu-id="79fad-123">名前</span><span class="sxs-lookup"><span data-stu-id="79fad-123">Name</span></span>      |<span data-ttu-id="79fad-124">説明</span><span class="sxs-lookup"><span data-stu-id="79fad-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="79fad-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="79fad-125">Authorization</span></span>  | <span data-ttu-id="79fad-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="79fad-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="79fad-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="79fad-127">Request body</span></span>
<span data-ttu-id="79fad-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79fad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79fad-129">応答</span><span class="sxs-lookup"><span data-stu-id="79fad-129">Response</span></span>
<span data-ttu-id="79fad-130">成功した場合、このメソッド`200 OK`は応答コードと、型`application/octet-stream`のコンテンツを返します。</span><span class="sxs-lookup"><span data-stu-id="79fad-130">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="79fad-131">例</span><span class="sxs-lookup"><span data-stu-id="79fad-131">Example</span></span>
<span data-ttu-id="79fad-132">この例では、すべての役割の割り当てを、Wingtip Toys のサブスクリプションの .csv ファイルとして保存します。</span><span class="sxs-lookup"><span data-stu-id="79fad-132">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="79fad-133">要求</span><span class="sxs-lookup"><span data-stu-id="79fad-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="79fad-134">応答</span><span class="sxs-lookup"><span data-stu-id="79fad-134">Response</span></span>
<span data-ttu-id="79fad-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="79fad-135">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
