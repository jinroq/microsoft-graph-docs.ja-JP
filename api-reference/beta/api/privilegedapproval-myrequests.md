---
title: 'privilegedApproval: myRequests'
description: 要求側の承認の要求を取得します。
localization_priority: Normal
ms.openlocfilehash: 9fcbdab424c98633a8f543875b9b7c2275894df0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512893"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="ab0c1-103">privilegedApproval: myRequests</span><span class="sxs-lookup"><span data-stu-id="ab0c1-103">privilegedApproval: myRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab0c1-104">要求側の承認の要求を取得します。</span><span class="sxs-lookup"><span data-stu-id="ab0c1-104">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab0c1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ab0c1-105">Permissions</span></span>
<span data-ttu-id="ab0c1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab0c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ab0c1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab0c1-108">Permission type</span></span>      | <span data-ttu-id="ab0c1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab0c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab0c1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab0c1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab0c1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ab0c1-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ab0c1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab0c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab0c1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab0c1-113">Not supported.</span></span>    |
|<span data-ttu-id="ab0c1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab0c1-114">Application</span></span> | <span data-ttu-id="ab0c1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab0c1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab0c1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ab0c1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="ab0c1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab0c1-117">Request headers</span></span>
| <span data-ttu-id="ab0c1-118">名前</span><span class="sxs-lookup"><span data-stu-id="ab0c1-118">Name</span></span>       | <span data-ttu-id="ab0c1-119">説明</span><span class="sxs-lookup"><span data-stu-id="ab0c1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab0c1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab0c1-120">Authorization</span></span>  | <span data-ttu-id="ab0c1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ab0c1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab0c1-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ab0c1-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ab0c1-124">応答</span><span class="sxs-lookup"><span data-stu-id="ab0c1-124">Response</span></span>

<span data-ttu-id="ab0c1-125">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[privilegedApproval](../resources/privilegedapproval.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ab0c1-125">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="ab0c1-126">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="ab0c1-126">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ab0c1-127">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="ab0c1-127">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="ab0c1-128">例</span><span class="sxs-lookup"><span data-stu-id="ab0c1-128">Example</span></span>
<span data-ttu-id="ab0c1-129">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ab0c1-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ab0c1-130">要求</span><span class="sxs-lookup"><span data-stu-id="ab0c1-130">Request</span></span>
<span data-ttu-id="ab0c1-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ab0c1-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```

##### <a name="response"></a><span data-ttu-id="ab0c1-132">応答</span><span class="sxs-lookup"><span data-stu-id="ab0c1-132">Response</span></span>
<span data-ttu-id="ab0c1-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ab0c1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-myrequests.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
