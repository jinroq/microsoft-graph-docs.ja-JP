---
title: privilegedRoleAssignment の削除
description: privilegedRoleAssignment を削除します。
localization_priority: Normal
ms.openlocfilehash: 2b98509457d7e26b4b65d42840f04550429bcc95
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546601"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="0d51d-103">privilegedRoleAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="0d51d-103">Delete privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d51d-104">[privilegedRoleAssignment](../resources/privilegedroleassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0d51d-104">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="0d51d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0d51d-105">Permissions</span></span>
<span data-ttu-id="0d51d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d51d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0d51d-108">リクエスターは、特権の_役割管理者_の役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d51d-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="0d51d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d51d-109">Permission type</span></span>      | <span data-ttu-id="0d51d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d51d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d51d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d51d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d51d-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d51d-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0d51d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d51d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d51d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d51d-114">Not supported.</span></span>    |
|<span data-ttu-id="0d51d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d51d-115">Application</span></span> | <span data-ttu-id="0d51d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d51d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d51d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d51d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="0d51d-118">ここで``<id>`` 、は ' userId_roleId ' の形式になっています。ここで、userId は azure AD ユーザー id の guid 文字列で、roleId は azure 管理者の役割 id の guid 文字列です。</span><span class="sxs-lookup"><span data-stu-id="0d51d-118">Note that ``<id>`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d51d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d51d-119">Request headers</span></span>
| <span data-ttu-id="0d51d-120">名前</span><span class="sxs-lookup"><span data-stu-id="0d51d-120">Name</span></span>       | <span data-ttu-id="0d51d-121">説明</span><span class="sxs-lookup"><span data-stu-id="0d51d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0d51d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d51d-122">Authorization</span></span>  | <span data-ttu-id="0d51d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0d51d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d51d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d51d-125">Request body</span></span>
<span data-ttu-id="0d51d-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0d51d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d51d-127">応答</span><span class="sxs-lookup"><span data-stu-id="0d51d-127">Response</span></span>

<span data-ttu-id="0d51d-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0d51d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="0d51d-130">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="0d51d-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="0d51d-131">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="0d51d-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="0d51d-132">例</span><span class="sxs-lookup"><span data-stu-id="0d51d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d51d-133">要求</span><span class="sxs-lookup"><span data-stu-id="0d51d-133">Request</span></span>
<span data-ttu-id="0d51d-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0d51d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="0d51d-135">応答</span><span class="sxs-lookup"><span data-stu-id="0d51d-135">Response</span></span>
<span data-ttu-id="0d51d-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0d51d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
