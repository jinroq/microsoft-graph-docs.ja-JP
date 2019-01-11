---
title: PrivilegedRoleAssignment を削除します。
description: PrivilegedRoleAssignment を削除します。
localization_priority: Normal
ms.openlocfilehash: 10d8b10522f26c386e918fb1806c1807d28314e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888943"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="c3dec-103">PrivilegedRoleAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="c3dec-103">Delete privilegedRoleAssignment</span></span>

> <span data-ttu-id="c3dec-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3dec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3dec-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3dec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3dec-106">[PrivilegedRoleAssignment](../resources/privilegedroleassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c3dec-106">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c3dec-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c3dec-107">Permissions</span></span>
<span data-ttu-id="c3dec-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3dec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c3dec-110">リクエスターでは、_ロールの権限を持つ管理者_のロールを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3dec-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="c3dec-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3dec-111">Permission type</span></span>      | <span data-ttu-id="c3dec-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3dec-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3dec-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3dec-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c3dec-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c3dec-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c3dec-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3dec-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3dec-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3dec-116">Not supported.</span></span>    |
|<span data-ttu-id="c3dec-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3dec-117">Application</span></span> | <span data-ttu-id="c3dec-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3dec-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3dec-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3dec-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="c3dec-120">注意してください``<id>``'userId_roleId'、Azure AD ユーザーの id の GUID の文字列は、ユーザー Id、roleId は、Azure の管理者ロールの id の GUID の文字列の形式にします。</span><span class="sxs-lookup"><span data-stu-id="c3dec-120">Note that ``<id>`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3dec-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3dec-121">Request headers</span></span>
| <span data-ttu-id="c3dec-122">名前</span><span class="sxs-lookup"><span data-stu-id="c3dec-122">Name</span></span>       | <span data-ttu-id="c3dec-123">説明</span><span class="sxs-lookup"><span data-stu-id="c3dec-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c3dec-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3dec-124">Authorization</span></span>  | <span data-ttu-id="c3dec-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c3dec-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3dec-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3dec-127">Request body</span></span>
<span data-ttu-id="c3dec-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3dec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3dec-129">応答</span><span class="sxs-lookup"><span data-stu-id="c3dec-129">Response</span></span>

<span data-ttu-id="c3dec-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c3dec-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="c3dec-132">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c3dec-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c3dec-133">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="c3dec-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c3dec-134">例</span><span class="sxs-lookup"><span data-stu-id="c3dec-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3dec-135">要求</span><span class="sxs-lookup"><span data-stu-id="c3dec-135">Request</span></span>
<span data-ttu-id="c3dec-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3dec-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="c3dec-137">応答</span><span class="sxs-lookup"><span data-stu-id="c3dec-137">Response</span></span>
<span data-ttu-id="c3dec-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3dec-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
