---
title: PrivilegedApproval を作成します。
description: この API を使用すると、新しい privilegedApproval を作成します。
localization_priority: Normal
ms.openlocfilehash: 076184417f6dc77dfc57046d75a3274716232f3b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507678"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="aba1f-103">PrivilegedApproval を作成します。</span><span class="sxs-lookup"><span data-stu-id="aba1f-103">Create privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aba1f-104">この API を使用すると、新しい privilegedApproval を作成します。</span><span class="sxs-lookup"><span data-stu-id="aba1f-104">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="aba1f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aba1f-105">Permissions</span></span>
<span data-ttu-id="aba1f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aba1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="aba1f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aba1f-108">Permission type</span></span>      | <span data-ttu-id="aba1f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aba1f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aba1f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aba1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aba1f-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aba1f-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aba1f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aba1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aba1f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aba1f-113">Not supported.</span></span>    |
|<span data-ttu-id="aba1f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aba1f-114">Application</span></span> | <span data-ttu-id="aba1f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aba1f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aba1f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aba1f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="aba1f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aba1f-117">Request headers</span></span>
| <span data-ttu-id="aba1f-118">名前</span><span class="sxs-lookup"><span data-stu-id="aba1f-118">Name</span></span>       | <span data-ttu-id="aba1f-119">説明</span><span class="sxs-lookup"><span data-stu-id="aba1f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aba1f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="aba1f-120">Authorization</span></span>  | <span data-ttu-id="aba1f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aba1f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aba1f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="aba1f-123">Request body</span></span>
<span data-ttu-id="aba1f-124">要求の本文には、 [privilegedApproval](../resources/privilegedapproval.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="aba1f-124">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aba1f-125">応答</span><span class="sxs-lookup"><span data-stu-id="aba1f-125">Response</span></span>

<span data-ttu-id="aba1f-126">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[privilegedApproval](../resources/privilegedapproval.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="aba1f-126">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="aba1f-127">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="aba1f-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="aba1f-128">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="aba1f-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="aba1f-129">例</span><span class="sxs-lookup"><span data-stu-id="aba1f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aba1f-130">要求</span><span class="sxs-lookup"><span data-stu-id="aba1f-130">Request</span></span>
<span data-ttu-id="aba1f-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aba1f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-type: application/json
Content-length: 180

{
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
<span data-ttu-id="aba1f-132">要求の本文には、 [privilegedApproval](../resources/privilegedapproval.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="aba1f-132">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="aba1f-133">応答</span><span class="sxs-lookup"><span data-stu-id="aba1f-133">Response</span></span>
<span data-ttu-id="aba1f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aba1f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 200

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
  "description": "Create privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-post-privilegedapproval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
