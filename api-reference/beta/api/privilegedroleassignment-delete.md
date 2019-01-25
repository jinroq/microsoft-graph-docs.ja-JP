---
title: PrivilegedRoleAssignment を削除します。
description: PrivilegedRoleAssignment を削除します。
localization_priority: Normal
ms.openlocfilehash: 2b98509457d7e26b4b65d42840f04550429bcc95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526747"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="46396-103">PrivilegedRoleAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="46396-103">Delete privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46396-104">[PrivilegedRoleAssignment](../resources/privilegedroleassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="46396-104">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="46396-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="46396-105">Permissions</span></span>
<span data-ttu-id="46396-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46396-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="46396-108">リクエスターでは、_ロールの権限を持つ管理者_のロールを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="46396-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="46396-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="46396-109">Permission type</span></span>      | <span data-ttu-id="46396-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="46396-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46396-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="46396-111">Delegated (work or school account)</span></span> | <span data-ttu-id="46396-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="46396-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="46396-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="46396-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46396-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46396-114">Not supported.</span></span>    |
|<span data-ttu-id="46396-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="46396-115">Application</span></span> | <span data-ttu-id="46396-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46396-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46396-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="46396-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="46396-118">注意してください``<id>``'userId_roleId'、Azure AD ユーザーの id の GUID の文字列は、ユーザー Id、roleId は、Azure の管理者ロールの id の GUID の文字列の形式にします。</span><span class="sxs-lookup"><span data-stu-id="46396-118">Note that ``<id>`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46396-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46396-119">Request headers</span></span>
| <span data-ttu-id="46396-120">名前</span><span class="sxs-lookup"><span data-stu-id="46396-120">Name</span></span>       | <span data-ttu-id="46396-121">説明</span><span class="sxs-lookup"><span data-stu-id="46396-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="46396-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="46396-122">Authorization</span></span>  | <span data-ttu-id="46396-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="46396-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46396-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="46396-125">Request body</span></span>
<span data-ttu-id="46396-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="46396-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46396-127">応答</span><span class="sxs-lookup"><span data-stu-id="46396-127">Response</span></span>

<span data-ttu-id="46396-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="46396-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="46396-130">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="46396-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="46396-131">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="46396-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="46396-132">例</span><span class="sxs-lookup"><span data-stu-id="46396-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46396-133">要求</span><span class="sxs-lookup"><span data-stu-id="46396-133">Request</span></span>
<span data-ttu-id="46396-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="46396-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="46396-135">応答</span><span class="sxs-lookup"><span data-stu-id="46396-135">Response</span></span>
<span data-ttu-id="46396-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="46396-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
