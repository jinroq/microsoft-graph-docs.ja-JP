---
title: 'privilegedRole: selfDeactivate'
description: リクエスターに割り当てられているロールを非アクティブ化します。
localization_priority: Normal
ms.openlocfilehash: 7175af64e7e36087bd048cd6e160393e2bf6377e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528691"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="31b52-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="31b52-103">privilegedRole: selfDeactivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31b52-104">リクエスターに割り当てられているロールを非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="31b52-104">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="31b52-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="31b52-105">Permissions</span></span>
<span data-ttu-id="31b52-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31b52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="31b52-108">リクエスターは呼び出すことができますのみ```selfDeactivate```彼に割り当てられているロールです。</span><span class="sxs-lookup"><span data-stu-id="31b52-108">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="31b52-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31b52-109">Permission type</span></span>      | <span data-ttu-id="31b52-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="31b52-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31b52-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31b52-111">Delegated (work or school account)</span></span> | <span data-ttu-id="31b52-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31b52-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="31b52-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31b52-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31b52-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31b52-114">Not supported.</span></span>    |
|<span data-ttu-id="31b52-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31b52-115">Application</span></span> | <span data-ttu-id="31b52-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31b52-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31b52-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31b52-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="31b52-118">注意してください``<id>``は、ターゲットのロールの id。</span><span class="sxs-lookup"><span data-stu-id="31b52-118">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="31b52-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31b52-119">Request headers</span></span>
| <span data-ttu-id="31b52-120">名前</span><span class="sxs-lookup"><span data-stu-id="31b52-120">Name</span></span>       | <span data-ttu-id="31b52-121">説明</span><span class="sxs-lookup"><span data-stu-id="31b52-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="31b52-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31b52-122">Authorization</span></span>  | <span data-ttu-id="31b52-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="31b52-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31b52-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="31b52-125">Request body</span></span>
<span data-ttu-id="31b52-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="31b52-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31b52-127">応答</span><span class="sxs-lookup"><span data-stu-id="31b52-127">Response</span></span>

<span data-ttu-id="31b52-128">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[privilegedRoleAssignment](../resources/privilegedroleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="31b52-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="31b52-129">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="31b52-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="31b52-130">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="31b52-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="31b52-131">例</span><span class="sxs-lookup"><span data-stu-id="31b52-131">Example</span></span>
<span data-ttu-id="31b52-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="31b52-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="31b52-133">要求</span><span class="sxs-lookup"><span data-stu-id="31b52-133">Request</span></span>
<span data-ttu-id="31b52-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="31b52-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```

##### <a name="response"></a><span data-ttu-id="31b52-135">応答</span><span class="sxs-lookup"><span data-stu-id="31b52-135">Response</span></span>
<span data-ttu-id="31b52-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="31b52-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-selfdeactivate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
