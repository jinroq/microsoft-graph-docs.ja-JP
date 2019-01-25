---
title: PrivilegedApproval を取得します。
description: プロパティと privilegedapproval オブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: c718c8d3c9382c5f8af9debf88fd6de5a55b461b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513621"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="37780-103">PrivilegedApproval を取得します。</span><span class="sxs-lookup"><span data-stu-id="37780-103">Get privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37780-104">プロパティと privilegedapproval オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="37780-104">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="37780-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="37780-105">Permissions</span></span>
<span data-ttu-id="37780-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37780-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="37780-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37780-108">Permission type</span></span>      | <span data-ttu-id="37780-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="37780-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37780-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37780-110">Delegated (work or school account)</span></span> | <span data-ttu-id="37780-111">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="37780-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="37780-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37780-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37780-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37780-113">Not supported.</span></span>    |
|<span data-ttu-id="37780-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37780-114">Application</span></span> | <span data-ttu-id="37780-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37780-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37780-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37780-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="37780-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="37780-117">Optional query parameters</span></span>
<span data-ttu-id="37780-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="37780-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37780-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37780-119">Request headers</span></span>
| <span data-ttu-id="37780-120">名前</span><span class="sxs-lookup"><span data-stu-id="37780-120">Name</span></span>      |<span data-ttu-id="37780-121">説明</span><span class="sxs-lookup"><span data-stu-id="37780-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37780-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="37780-122">Authorization</span></span>  | <span data-ttu-id="37780-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="37780-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37780-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="37780-125">Request body</span></span>
<span data-ttu-id="37780-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="37780-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37780-127">応答</span><span class="sxs-lookup"><span data-stu-id="37780-127">Response</span></span>

<span data-ttu-id="37780-128">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[privilegedApproval](../resources/privilegedapproval.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="37780-128">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="37780-129">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="37780-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="37780-130">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="37780-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="37780-131">例</span><span class="sxs-lookup"><span data-stu-id="37780-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37780-132">要求</span><span class="sxs-lookup"><span data-stu-id="37780-132">Request</span></span>
<span data-ttu-id="37780-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="37780-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
##### <a name="response"></a><span data-ttu-id="37780-134">応答</span><span class="sxs-lookup"><span data-stu-id="37780-134">Response</span></span>
<span data-ttu-id="37780-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="37780-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
