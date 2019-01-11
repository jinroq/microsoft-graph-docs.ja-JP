---
title: 学生を削除する
description: educationClass から educationUser を削除する
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 0afab5c80c546a9404ee11fc4d127d15b13a4e9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824152"
---
# <a name="remove-a-student"></a><span data-ttu-id="b8d17-103">学生を削除する</span><span class="sxs-lookup"><span data-stu-id="b8d17-103">Remove a student</span></span>

> <span data-ttu-id="b8d17-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b8d17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8d17-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8d17-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8d17-106">[educationClass](../resources/educationclass.md) から [educationUser](../resources/educationuser.md) を削除する</span><span class="sxs-lookup"><span data-stu-id="b8d17-106">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="b8d17-107">**メモ:** 教師_および_学生は、クラス **members** コレクションに所属します。</span><span class="sxs-lookup"><span data-stu-id="b8d17-107">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="b8d17-108">この API を呼び出す前に、削除する **educationUser** が教師でないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b8d17-108">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="b8d17-109">[educationclass_list_teachers](educationclass-list-teachers.md) を呼び出して教師のリストを取得し、削除対象のユーザーのユーザー ID が返された教師リストにないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="b8d17-109">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8d17-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b8d17-110">Permissions</span></span>
<span data-ttu-id="b8d17-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8d17-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8d17-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b8d17-113">Permission type</span></span>      | <span data-ttu-id="b8d17-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8d17-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8d17-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8d17-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="b8d17-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8d17-116">Not supported.</span></span>  |
|<span data-ttu-id="b8d17-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8d17-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b8d17-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8d17-118">Not supported.</span></span>  |
|<span data-ttu-id="b8d17-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8d17-119">Application</span></span> | <span data-ttu-id="b8d17-120">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8d17-120">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b8d17-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8d17-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b8d17-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8d17-122">Request headers</span></span>
| <span data-ttu-id="b8d17-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8d17-123">Header</span></span>       | <span data-ttu-id="b8d17-124">値</span><span class="sxs-lookup"><span data-stu-id="b8d17-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8d17-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8d17-125">Authorization</span></span>  | <span data-ttu-id="b8d17-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b8d17-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8d17-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8d17-128">Request body</span></span>
<span data-ttu-id="b8d17-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b8d17-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b8d17-130">応答</span><span class="sxs-lookup"><span data-stu-id="b8d17-130">Response</span></span>
<span data-ttu-id="b8d17-131">成功した場合、このメソッドは `204 No Content` 応答コードと空の応答本文を返します。</span><span class="sxs-lookup"><span data-stu-id="b8d17-131">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8d17-132">例</span><span class="sxs-lookup"><span data-stu-id="b8d17-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8d17-133">要求</span><span class="sxs-lookup"><span data-stu-id="b8d17-133">Request</span></span>
<span data-ttu-id="b8d17-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8d17-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11003/members/14008
```

##### <a name="response"></a><span data-ttu-id="b8d17-135">応答</span><span class="sxs-lookup"><span data-stu-id="b8d17-135">Response</span></span>
<span data-ttu-id="b8d17-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8d17-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
